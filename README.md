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
