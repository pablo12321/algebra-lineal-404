# Capítulo 3: Determinante

## 3.1 Definición y propiedades

El determinante es un __número__ especial y __único__ que se asocia a una matriz cuadrada.

Sea $S_3 = \{1,2,...,n\}$ el conjunto de enteros de 1 a $n$, ordenados en forma ascendente. Un reordenamiento $j_1,j_2,...,j_n$ de los números es una permutación de S. Hay un total de $n!$(n factorial) permutaciones de $S$.

Una permutacion de $S$, $j_1,j_2,...,j_n$ tiene una __inversión__, si un entero mayor se ubica antes de un entero menor. Una permutación se denomina par o impar si el numero total de inversiones es par o impar respectivamente.

Ejemplo:

Sea $S_3= \{1,2,3\}$, $j_1,j_2,j_3 = 312$, es una permutación de $S_3$.

Hay $3! = 6$ permutaciones totales en $S_3$

Las permutaciones pares son:
  
  - 123 (0 inversiones)
  - 231 (21,31)
  - 312 (31,32)

Y las imapres:

  - 132 (32)
  - 213 (21)
  - 321(32,31,21)

__Definición__:

Sea $A$ una matriz de nxn, el determinante de $A$ denotado por $det(A)$ o $|A|$, es:
$$
|A| = a_{1_{j1}}+a_{2_{j2}}+...+a_{n_{jn}}
$$
donde la suma varíasobre todas las permutaciones y el signo es $+$ si la permutación es par o $-$si es impar.

### Matrices de 2x2
$$

  A=
  \left[ {\begin{array}{cc}
   1 & 2 \\
   3 & 4 
  \end{array}} \right];
  S_2=\{ 1,2\}
$$

Permutaciones totales: 2: 12 y 21. 
$$|A| = a_{1-}a_{2-} - a_{1-}a_{2-}$$
$$|A| = a_{11}a_{22} - a_{12}a_{21}$$

### Matrices de 3x3
Hay $3!=6$ permutaciones totales:

Las pares son: 123, 231, 312 \
Las impares son: 132, 213, 321

$|A| = a_{1-}a_{2-}a_{3-}+a_{1-}a_{2-}a_{3-}+a_{1-}a_{2-}a_{3-}$
$- a_{1-}a_{2-}a_{3-} - a_{1-}a_{2-}a_{3-} - a_{1-}a_{2-}a_{3-}$

\
$|A| = a_{11}a_{22}a_{33}+a_{12}a_{23}a_{31}+a_{13}a_{21}a_{32}$
$- a_{11}a_{23}a_{32} - a_{12}a_{21}a_{33} - a_{13}a_{22}a_{31}$
___
### Propiedades de los determinantes
### Teorema 3.1
Los determinantes de una matriz y su transpuesta son iguales, es decir, $|A| = |A^T|$.

### Teorema 3.2

Si la matriz $B$ se obtiene de la matriz $A$ al intercambiar dos filaso columnas de $A$, entonces $|B| = -|A|$.

### Teorema 3.3
Si $A$ tiene dos filas o columnas iguales, entonces $|A| = 0$.

### Teorema 3.4
Si una fila o columna de $A$ es cero, entonces  $|A| = 0$.

### Teorema 3.5
Si la matriz $B$ se obtiene de la matriz $A$ al multiplicar una fila o columna por un escalar $a$, entonces $|B| = a|A|$.


 > Observación:\
 > Si cada una de las $n$ filas de $aA$ tiene un factor común $a$, se sabe que $|aA| = a^n|A|$

### Teorema 3.6
Si la matriz $B$ se obtiene de sumar o restar de una fila o columna de $A$ un múltiplo de otra, entonces $|B| = |A|$

### Teorema 3.7
Si una matriz es triangular el determinante es el producto de las entradas de la diagonal principal.

### Teorema 3.8
El determinante del producto de dos matrices es el producto de sus determinantes, es decir, $|AB| = |A|.|B|$
___
## 3.2 Desarrollo por cofactores
Sea $A$ una matriz de nxn y sean $M_{ij}$ las submatrices de (n-1)x(n-1) obtenidas al eliminar la i-esima fila y la j-esima columna de $A$. El determinante, $|M_{ij}|$ es el menor de $a_{ij}$ y el cofactor $A_{ij}$ de $a_{ij}$ es:

$$
  A_{ij} = (-1).|M_{ij}|
$$
### Teorema 3.9
Sea $A$ una matriz de nxn, entonces para cada $i$ el desarrollo de $|A|$ a lo largo de la i-esima fila es:
$$
|A| = a_{i1}A_{i1}+a_{i2}A_{i2}+...+a_{in}A_{in}
$$
Donde $A{ij}$ es el cofactor de $a_{ij}$

De manera similar se puede obtener por cofactores de la j-esima columna de $A$
$$
|A| = a_{1j}A_{1j}+a_{2j}A_{2j}+...+a_{nj}A_{nj}
$$

### La inversa de una matriz
Sea $A$ una matriz de nxn, la matriz de nxn $\text {adj} A$, llamada la **adjunta** de $A$. es la matriz cuyo i,j-esimo elemento es el cofactor $A_{ij}$ de $a_{ij}$.
$$
  \text {adj } A=
  \left[ {\begin{array}{ccc}
   A_{11} & A_{21} & A_{31} \\
   A_{21} & A_{22} & A_{23} \\
   A_{31} & A_{32} & A_{33}
  \end{array}} \right]
$$

___
### Teorema 3.12
Una matriz $A$ es **no singular**, si y solo si, $|A| <> 0$.\
Por el contrario, si $A$ es **singular**, entonces $|A| = 0$
___
### Lista de equivalencias no signulares
1. $A$ es no singular.
2. $A$ es equivalente por filas a $I_n$
3. $Ax = 0$ solo tiene solución trivial.
4. $Ax = b$ tiene solucion unica para cada b.
5. $|A| <> 0$