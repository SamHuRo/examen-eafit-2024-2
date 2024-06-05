# Examen de la universidad EAFIT para 2024-2

## Pregunta 1

Una empresa vende un producto en un mercado competitivo y desea determinar el precio óptimo de venta para maximizar sus ganancias. La demanda del producto, el costo de producción y la ganancia de la empresa están influenciadas por el precio de venta y se han modelado de la siguiente forma:

* **Función de demanda:** la cantidad de demanda $q(p)$ del producto depende del precio $p$ según la realción:

$$
q(p) = 500 - 2p
$$

* **Costo de producción:** el costo de producir una unidad del producto es constante y es de $20 por unidad

* **Función de ingreso total:** el ingreso total $R(p)$ se calcula multipliacando el precio del oroducto por la cantidad demanda:

$$
R(p) = p*q(p)
$$

* **Función de costo total:** El costo total $C$ de producir $q$ unidades es:

$$
C(p) = 20 q(p)
$$

* **Función de ganancia:** la ganancia $G(p)$ se calcula como el ingreso total menos el costo total:

$$
G(p) = R(p) - C(p)
$$

### Ejercicio:

* Defina la función de ganancia en función del precio del producto.
* Encuentre el precio $p$ que maximiza la función del costo total $G(p)$.
    * Maximice la función utilizando una solución analítica.
    * Macimice la función utilizando gradiente ascendente.
    * Grafique la función y corrobore que el punto máximo encontrado corresponde al máximo de la función.

## Pregunta 2

Se han registrado los siguientes datos que muestran la realación entre la cantidad de luz solar diaria (horas) y la altura de las plantas (cm) en un experimento de cultivo:

| Luz Solar [horas]        | Altura de la planta [cm]|
|--------------------------|-------------------------|
| 2                        | 5                       |
| 3                        | 7                       |
| 5                        | 10                      |
| 6                        | 13                      |
| 8                        | 15                      |
| 9                        | 18                      |

Se desea encontrar la mejor recta $y = \beta_{0} + \beta{1}*x$ que se ajuste a estos datos utilizando la ecuación normal de mínimos cuadrados para predecir la altura de las plantas en función de la cantidad de luz solar: 

### Ejercicios:

* Plnatee la ecuación normal $\beta = (X^{T} X)^{-1} X^{T} Y$ donde
    * $X$ es una matriz de $n \times 2$ tal que su primera columna consiste en unos y la segunda columna está conformada por los $n$ valores de la variables independiente.
    * $Y$ es una matriz $n \times 1$ conformada por los valores de la variable dependiente.
    * $\beta$ es una matriz $n \times 1$ cuyas entradas son $\beta_{0}$, $\beta_{1}$, ..., $\beta_{n}$
* Encuentre manualmente los coeficientes $\beta_{0}$ y $\beta_{1}$ usando la ecuación normal.
* Implemente una solución computacional que verifique el resultado obtenido manualmente.
* Grafique el conjunto de datos suministrado junto con la línea recta ajustada.

## Pregunta 3

Se ha registrado el consumo de energía eléctrica en kilovatios-hopa (kWh) en un edificio de oficinas cada hora durante un día laborable. los datos se encuentran en el archivo "consumo_energia.csv".

1. Estadísticas descriptivas
    * Calcule la media, la mediana, la moda y la desviación estándar del consumo de energía eléctrica por hora
2. Análisis de datos
    * Calcule el primer y tercer cuartil e interprete los resultados obtenidos.
3. Evaluación de consumo
    * Si se considera que un consumo de más de 100 kWhpor hora es alto ¿cuál es la proporción de horas que tienen un consumo alto?.
    * Basándose en la media y la mediana, ¿qué puede decir sobre la distribución del consumo de energía eléctrica oir hora?.
4. Planificación de recursos
    * Si se planea implementar medidas de ahorro de energía durante las horas de alto consumo, ¿cuántas horas al día sería necesario implementar estas medidas?
    * Si el costo de operación adicional por hora para implementar medidas de ahorro es de $50 durante las horas de alto consumo, estime el costo adicional para un día laborable.
5. Visualización de datos
    * Genere un histograma que represente el consumo de energía eléctrica por hora en el edificio de oficinas. Identifique los periodos de alto y bajo consumo.

## Pregunta 4

El archivo "datos_multivariados.csv" contiene un conjunto de datos con 10 variables y 100 observaciones que describen un determinado fenómeno. En particular, las variables presentan diferentes distribuciones y algunas contienen valores atípicos (outliers). Además, ciertas variables están correlacionadas entre si.

1. Visualización preliminar de datos
    * Genere gráficas de dispersión (scatter plot) para examinar las relaciones entre variables.
    * Genere diagramas de caja (box plots) para evidenciar la presencia de outliers.
    * Genere histogramas para entender la distribución de cada variable.
2. Identificación y eliminación de outliers
    * Utilice el rango intercuartílico (IQR) para identificar y eliminar las observaciones que contienen al menos un valor atípico en cualquier variable.
    * Documente el número de observaciones eliminadas y el conjunto de datos resultante.
3. Correlación de datos
    * Calcule la matriz de correlación de Pearson para las variables del conjunto de datos limpio.
    * Visualice la matriz de correlación utilizando un mapa de calor (heatmap).
4. Selección de varialbes no correlacionadas
    * Establezca un umbral de correlación (por ejemplo, 0.7).
    * Identifique los pares de variables cuya correlación absoluta exceda el umbral establecido.
    * Retenga todas las variables que no superen el umbral de correlación. Para cada par de variables que lo superen, seleccione la variable que muestre una mayor dispersión de los datos, ya que es problable que contenga más información relevante sobre el fenómeno que se está estudiando.
    * Obtenga un conjunto final de datos con las variables seleccionadas.
