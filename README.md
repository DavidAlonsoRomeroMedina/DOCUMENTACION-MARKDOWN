# Documentación de Ejercicios - David Alonso Romero Medina

## Información General
- **Materia:** Fundamentos de Álgebra
- **Tema:** Determinantes, Regla de Sarrus y Cofactores
- **Fecha:** 18 de Noviembre de 2025
- **Estudiante:** David Alonso Romero Medina
- **Grupo:** 1C

## Objetivo de la Documentación
Documentar la resolución de ejercicios prácticos sobre álgebra lineal, incluyendo el cálculo de determinantes de $2\times2$ y $3\times3$ mediante diferentes métodos (definición, Sarrus y Cofactores), verificación de propiedades de matrices y aplicaciones geométricas.

---

## Ejercicios Realizados

### Ejercicio 1: Determinantes de $2\times2$

#### Enunciado del Problema
Calcular el determinante de las siguientes matrices:

$$ A =
\begin{pmatrix}
5 & 2 \\
3 & 1 \\
\end{pmatrix}
$$

$$ B =
\begin{pmatrix}
-1 & 4 \\
2 & -8 \\
\end{pmatrix}
$$

$$ C =
\begin{pmatrix}
6 & 9 \\
2 & 3 \\
\end{pmatrix}
$$

#### Solución o Respuesta
1. **Det(A)** = -1
2. **Det(B)** = 0
3. **Det(C)** = 0

#### Proceso/Procedimiento
Para calcular un determinante de $2\times2$, multiplicamos la diagonal principal y restamos el producto de la diagonal secundaria.

**1. Matriz A:**
$$(5)(1) - (2)(3) = 5 - 6 = -1$$

**2. Matriz B:**
$$(-1)(-8) - (4)(2) = 8 - 8 = 0$$

**3. Matriz C:**
$$(6)(3) - (9)(2) = 18 - 18 = 0$$


### Ejercicio 2: Regla de Sarrus (Matrices $3\times3$)

#### Enunciado del Problema
Calcular el determinante de las matrices E y F:

$$ E =
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 4 \\
5 & 6 & 0 \\
\end{pmatrix}
$$

$$ F =
\begin{pmatrix}
2 & -1 & 3 \\
1 & 4 & 0 \\
3 & 2 & -2 \\
\end{pmatrix}
$$

#### Solución o Respuesta
- **Det(E)** = 1
- **Det(F)** = -48

#### Proceso/Procedimiento
**Para la Matriz E:**
1. **Diagonales descendentes (+):**
$$(1)(1)(0) + (2)(4)(5) + (3)(0)(6) = 0 + 40 + 0 = 40$$

2. **Diagonales ascendentes (-):**
$$(5)(1)(3) + (6)(4)(1) + (0)(0)(2) = 15 + 24 + 0 = 39$$

3. **Resultado:**
$$40 - 39 = 1$$


### Ejercicio 3: Método de Cofactores

#### Enunciado del Problema
Calcular el determinante de la matriz G usando cofactores:

$$ G =
\begin{pmatrix}
1 & 0 & 2 \\
-1 & 3 & 1 \\
2 & 0 & 1 \\
\end{pmatrix}
$$

#### Solución o Respuesta
El determinante es **-9**.

#### Proceso/Procedimiento
Se eligió la **Fila 1** por contener un cero.

$$ det(G) = 1 \cdot
\begin{vmatrix}
3 & 1 \\
0 & 1 \\
\end{vmatrix}
$$


$$ - 0 + 2 \cdot
\begin{vmatrix}
-1 & 3 \\
2 & 0 \\
\end{vmatrix}
$$

$$det(G) = 1(3) + 2(-6)$$

$$det(G) = 3 - 12 = -9$$


### Ejercicio 4: Propiedades de los Determinantes

#### Enunciado
Dadas las matrices A y B:

$$ A =
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix}
$$

$$ B =
\begin{pmatrix}
1 & 2 \\
3 & 1 \\
\end{pmatrix}
$$

Verificar que $det(AB) = det(A) \cdot det(B)$.

#### Solución
1. **Calculamos individuales:**
   - Det(A) = $6 - 1 = 5$
   - Det(B) = $1 - 6 = -5$
   - Producto: $5 \times -5 = -25$

2. **Calculamos matriz AB:**

$$ AB =
\begin{pmatrix}
5 & 5 \\
10 & 5 \\
\end{pmatrix}
$$

3. **Determinante de AB:**
   - $25 - 50 = -25$

**Conclusión:** La propiedad se cumple ($-25 = -25$).

### Ejercicio 5: Aplicación Geométrica

#### Enunciado
Calcular el área del paralelogramo formado por los vectores:

$$\vec{v} = (3, 2)$$
$$\vec{w} = (1, 4)$$

#### Solución
El área es **10 u²**.

#### Proceso
Colocamos los vectores en una matriz y calculamos el determinante:

$$ Area = det
\begin{pmatrix}
3 & 2 \\
1 & 4 \\
\end{pmatrix}
$$

$$(3)(4) - (2)(1) = 12 - 2 = 10$$

El valor absoluto del determinante es el área.



---







