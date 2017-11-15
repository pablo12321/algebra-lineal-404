# Capitulo 4: Vectores en $R^n$

## 4.2 n-vectores
Un n-vecto en $R^n$ o n-vector es una matriz de nx1

$$
\vec{u}= \left[ {\begin{array}{cc}
 u_1\\
 u_2\\
 ...\\
 u_n
 \end{array}} \right] 
$$

Donde $u_1,u_2,...,u_n$ son numero reales, componentes de $\vec{u}$. El conjunto de todos los n-vectores se denota por $R^n$ y se llama n-espacio.
___
### Operaciones con vectores
Recordando que los vectores son matrices, las reglas para operar entre vectores son las que se definen anteriormente.

#### Suma de vectores
si $\vec{u}$ y $\vec{v}$ son vectores de $R^n$, entonces la suma es

$$
\vec{u}+\vec{v}= \left[ {\begin{array}{cc}
 u_1+v_1\\
 u_2+v_2\\
 ...\\
 u_n+v_n
 \end{array}} \right] 
$$

#### Multiplicación escalar
Si $\vec{u}$ es un vector de $R^n$ y $c$ es un escalar, entonces $c\vec{u}$ es un vector de $R^n$, donde
$$
c\vec{u}= \left[ {\begin{array}{cc}
 cu_1\\
 cu_2\\
 ...\\
 cu_n
 \end{array}} \right] 
$$

$c\vec{u}$ es un vector **co-lineal** con $\vec{u}$, cuya magnitud y sentido dependeran del escalar $c$.
___
La suma y multiplicación satisfacen las siguientes propiedades

#### Teorema 4.2
Sean $\vec{u}$,$\vec{v}$,$\vec{w}$ vectores cualesquiera de $R^n$, sean $c$ y $d$ escalares. Entonces $\vec{u}+\vec{v}$ es un vector de $R^n$.

$R^n$ es cerrado bajo la operacion suma.
1. $\vec{u}+\vec{v} = \vec{v}+\vec{u}$
2. $\vec{u}+(\vec{v}+\vec{w}) = (\vec{u}+\vec{v})+\vec{w}$
3. $\vec{u}+0 = 0+\vec{u} = 0$, Existe un 0 para todo $\vec{u}$ en $R^n$
4. $\vec{u}+(-\vec{u}) = 0$, Existe un $-\vec{u}$ para cada $\vec{u}$ en $R^n$

$c\vec{u}$ es un vector en $R^n$. 

$R^n$ es cerrado bajo la operación de la multiplicación por un escalar.

5. $c(\vec{u}+\vec{v}) = cv + c\vec{u}$
6. $(c+d)\vec{u} = c\vec{u} + d\vec{u}$
7. $c(d\vec{u}) = (cd)\vec{u}$
8. $1\vec{u} = \vec{u}$

#### Producto punto en $R^n$
La longitud del vector $\vec{u}$ en $R^n$ es

$$
|\vec{u}| = \sqrt{u_1^2+u_2^2+...+u_n^2}
$$

La distancia entre dos puntos $\vec{u}$ y $\vec{v}$ se define como la longitud del vector $|\vec{u} -\vec{v}|$ .
$$
 \text d(\vec u,\vec v) = |\vec u - \vec v|
$$
El producto punto entre dos vectores en $R^n$ es:
$$
u= \left[ {\begin{array}{cc}
 u_1\\
 u_2\\
 ...\\
 u_n
 \end{array}} \right] \text { ; } 
 v= \left[ {\begin{array}{cc}
 v_1\\\text{cos } \theta =
 v_2\\
 ...\\
 v_n
 \end{array}} \right]
$$
$$
\vec u.\vec v = u_1v_1,u_2v_2,...,u_nv_n
$$
#### Teorema 4.3 - Propiedades del producto punto
Si $\vec u$,$\vec v$,$\vec w$ son vectores en $R^n$ y $c$ es un escalar, entonces
1. $\vec u.\vec u > 0$ para $\vec u <> 0$; $\vec u.\vec u = 0$  si y solo si $\vec u = 0$
2. $\vec u.\vec v = \vec v.\vec u$ 
3. $(\vec u+\vec v).\vec w = \vec u.\vec w+\vec v.\vec w$ 
4. $(c\vec u).\vec v = \vec u.(c\vec v)=\vec c.(u\vec v)$ 

Si $\vec u$ y $\vec v$ son vectores distintos de cero, el coseno del angulo entre ellos es:
$$
\text {cos }\theta = \frac {\vec u.\vec v}{|\vec u|.|\vec v|}
$$
Decimos que son paralelos cuando $|\vec u|.|\vec v| = |\vec u.\vec v|$ porque $\text{cos } \theta = +1 \text { o}-1$

Son ortogonales cuando $\text{cos } \theta = 0$

#### Producto cruz
Si $\vec u$ y $\vec v$ son dos vectores en $R^3$ se puede usar la tecnica de
$$
\vec{u}\times\vec{v}= \left[ {\begin{array}{ccc}
 i & j & k\\
 u_1 & u_2 & u_3\\
 v_1 & v_2 & v_3
 \end{array}} \right] 
$$
