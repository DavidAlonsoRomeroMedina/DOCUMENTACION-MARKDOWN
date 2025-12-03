# Tecnológico de Software
## Materia: Fundamentos de álgebra
## 3/12/2025
## Alumno: Astrit Airan Cetzal Cetzal
## Actividad \#22 - Matrices

----
### Para esta actividad resolvimos ejercicios que implican matrices, esto con el fin de documentarlo. Apartir de varios metodos (Gauss, Gauss Jordan,inversa, Cramer) encontramos los valores de X, Y y Z . 

### Ejercicio 1: Resolver con todos los metodos 

##### Gaus 

$$
\begin{Bmatrix}
x & + y & + z\\ =6 \\
2x & -y & + z\\ =3 \\
x & 2y & -z\\ =2 \\
\end{Bmatrix}
$$

$$ A=
\begin{bmatrix}
1 & 1 & 1\\
2 & -1 & 1\\
1 & 2 & -1\\
\end{bmatrix}
$$ 

$$ B=
\begin{bmatrix}
-1 \\
3 \\
2 \\
\end{bmatrix}
$$

- Matriz aumentada

$$
\begin{bmatrix}
1 & 1 & 1\\
2 & -1 & 1\\
1 & 2 & -1\\
\end{bmatrix}
\begin{bmatrix}
-1 \\
3 \\
2 \\
\end{bmatrix}
$$

R2 -> -2R1 +R2
R3 -> -2R1 +R3

$$
\begin{pmatrix}
1 & 1 & 1\\
0 & -3 & -1\\
0 & 1 & -2\\
\end{pmatrix}
\begin{pmatrix}
6 \\
-9 \\
2 \\
\end{pmatrix}
$$

-1/3R2

$$
\begin{pmatrix}
1 & 1 & 1\\
0 & 1 & -1/3\\
0 & 1 & -2\\
\end{pmatrix}
\begin{pmatrix}
6 \\
3 \\
-4 \\
\end{pmatrix}
$$

R3 -> -R2 + R3

$$
\begin{pmatrix}
1 & 1 & 1\\
0 & 1 & 1/3\\
0 & 0 & -7/3\\
\end{pmatrix}
\begin{pmatrix}
6 \\
3 \\
-7 \\
\end{pmatrix}
$$

x + y + z =6 \
y + 1/3z=3 \
-7/3=-7 

-7/3z = -7 \
z= -7/1/-7/3 \
z= 21/7 \
z=3 

y + 1/3z=3 \
y + 1/3(3)=3 \
y + 1=3 \
y=3-1 \
y=2 

x + y + z =6 \
x + 2 + 3= 6 \
x + 5 = 6 \
x = 6 -5 \
x = 1 

Comprobación
1+ 2 + 3 =6


2. Gauss jordan
$$ A=
\begin{bmatrix}
1 & 1 & 1\\
2 & -1 & 1\\
1 & 2 & -1\\
\end{bmatrix}
$$ 

$$ B=
\begin{bmatrix}
-1 \\
3 \\
2 \\
\end{bmatrix}
$$

- Matriz aumentada

$$
\begin{bmatrix}
1 & 1 & 1\\
2 & -1 & 1\\
1 & 2 & -1\\
\end{bmatrix}
\begin{bmatrix}
-1 \\
3 \\
2 \\
\end{bmatrix}
$$

R2 -> -2R1 +R2
R3 -> -2R1 +R3

$$
\begin{pmatrix}
1 & 1 & 1\\
0 & -3 & -1\\
0 & 1 & -2\\
\end{pmatrix}
\begin{pmatrix}
6 \\
-9 \\
2 \\
\end{pmatrix}
$$

-1/3R2

$$
\begin{pmatrix}
1 & 1 & 1\\
0 & 1 & -1/3\\
0 & 1 & -2\\
\end{pmatrix}
\begin{pmatrix}
6 \\
3 \\
-4 \\
\end{pmatrix}
$$

R1 -> -R2 + R1
R3 -> -R2 + R3

$$
\begin{pmatrix}
1 & 0 & 2/3\\
0 & 1 & 1/3\\
0 & 0 & -7/3\\
\end{pmatrix}
\begin{pmatrix}
3 \\
3 \\
-7 \\
\end{pmatrix}
$$

-7/3R3

$$
\begin{pmatrix}
1 & 0 & 2/3\\
0 & 1 & 1/3\\
0 & 0 & 1\\
\end{pmatrix}
\begin{pmatrix}
3 \\
3 \\
3 \\
\end{pmatrix}
$$

R1=-2/3R3 + R1
R2=-1/3R3 + R2

$$
\begin{pmatrix}
1 & 0 & 0\\
0 & 1 & 0\\
0 & 0 & 1\\
\end{pmatrix}
\begin{pmatrix}
1 \\
2 \\
3 \\
\end{pmatrix}
$$

X = 1 |
y = 2 |
z = 3

3. Inversa

4. Cramer

