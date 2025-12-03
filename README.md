# Cálculo de Matriz Inversa (Método Gauss-Jordan)

Este documento detalla el procedimiento paso a paso para encontrar la inversa de la matriz de coeficientes del siguiente sistema de ecuaciones lineales.

## 1. Definición del Problema

**Sistema de Ecuaciones:**

$$
\begin{cases}
x + y + z = 6 \\
2x - y + z = 3 \\
x + 2y - z = 2
\end{cases}
$$

**Matriz de Coeficientes ($A$):**

$$
A = 
\begin{bmatrix}
1 & 1 & 1 \\
2 & -1 & 1 \\
1 & 2 & -1
\end{bmatrix}
$$

---

## 2. Resultado Final

La matriz inversa $A^{-1}$ es:

$$
A^{-1} = \frac{1}{7}
\begin{bmatrix}
-1 & 3 & 2 \\
3 & -2 & 1 \\
5 & -1 & -3
\end{bmatrix}
$$

O en forma decimal/fraccionaria:

$$
A^{-1} = 
\begin{bmatrix}
-1/7 & 3/7 & 2/7 \\
3/7 & -2/7 & 1/7 \\
5/7 & -1/7 & -3/7
\end{bmatrix}
$$

---

## 3. Procedimiento Paso a Paso (Gauss-Jordan)

El objetivo es transformar la matriz aumentada $[A | I]$ hasta obtener $[I | A^{-1}]$.

### Paso 3.1: Matriz Aumentada Inicial

$$
\left[
\begin{array}{ccc|ccc}
1 & 1 & 1 & 1 & 0 & 0 \\
2 & -1 & 1 & 0 & 1 & 0 \\
1 & 2 & -1 & 0 & 0 & 1
\end{array}
\right]
$$

### Paso 3.2: Eliminación en la Columna 1

Hacemos ceros debajo del pivote de la fila 1 ($F_1$).
* $F_2 \rightarrow F_2 - 2F_1$
* $F_3 \rightarrow F_3 - F_1$

$$
\left[
\begin{array}{ccc|ccc}
1 & 1 & 1 & 1 & 0 & 0 \\
0 & -3 & -1 & -2 & 1 & 0 \\
0 & 1 & -2 & -1 & 0 & 1
\end{array}
\right]
$$

### Paso 3.3: Reordenamiento de Filas

Intercambiamos $F_2$ y $F_3$ para facilitar los cálculos (poniendo el 1 como pivote).
* $F_2 \leftrightarrow F_3$

$$
\left[
\begin{array}{ccc|ccc}
1 & 1 & 1 & 1 & 0 & 0 \\
0 & 1 & -2 & -1 & 0 & 1 \\
0 & -3 & -1 & -2 & 1 & 0
\end{array}
\right]
$$

### Paso 3.4: Eliminación en la Columna 2

Hacemos cero debajo del pivote de la fila 2.
* $F_3 \rightarrow F_3 + 3F_2$

$$
\left[
\begin{array}{ccc|ccc}
1 & 1 & 1 & 1 & 0 & 0 \\
0 & 1 & -2 & -1 & 0 & 1 \\
0 & 0 & -7 & -5 & 1 & 3
\end{array}
\right]
$$

### Paso 3.5: Normalización de la Fila 3

Dividimos $F_3$ entre $-7$ para obtener el pivote unitario.
* $F_3 \rightarrow F_3 / -7$

$$
\left[
\begin{array}{ccc|ccc}
1 & 1 & 1 & 1 & 0 & 0 \\
0 & 1 & -2 & -1 & 0 & 1 \\
0 & 0 & 1 & 5/7 & -1/7 & -3/7
\end{array}
\right]
$$

### Paso 3.6: Sustitución hacia atrás (Hacer ceros arriba)

Eliminamos los elementos por encima de los pivotes principales.

**Usando $F_3$ para limpiar Columna 3:**
* $F_2 \rightarrow F_2 + 2F_3$
* $F_1 \rightarrow F_1 - F_3$

$$
\left[
\begin{array}{ccc|ccc}
1 & 1 & 0 & 2/7 & 1/7 & 3/7 \\
0 & 1 & 0 & 3/7 & -2/7 & 1/7 \\
0 & 0 & 1 & 5/7 & -1/7 & -3/7
\end{array}
\right]
$$

**Usando $F_2$ para limpiar Columna 2:**
* $F_1 \rightarrow F_1 - F_2$

$$
\left[
\begin{array}{ccc|ccc}
1 & 0 & 0 & -1/7 & 3/7 & 2/7 \\
0 & 1 & 0 & 3/7 & -2/7 & 1/7 \\
0 & 0 & 1 & 5/7 & -1/7 & -3/7
\end{array}
\right]
$$

## 4. Verificación

Se cumple que $A \cdot A^{-1} = I$.
