# Palabras

## Definición

-   Palabra

    Sea $$A$$ un **alfabeto**. Una **palabra** en $$A$$ de longitud $$r$$ es
    una función $$f\colon[r]\to A$$. Escribimos la palabra $$f$$
    como $$f(1)f(2)\cdots f(r)$$.

-   Ejemplo

    Por ejemplo, si $$A=\{x,y,z\}$$, las palabras de longitud 2 son:
    
    $$
    xx,xy,xz,yx,yy,yz,zx,zy,zz.
    $$



-   Cantidad de palabras

    Si el alfabeto $$A$$ tiene $$n$$ elementos, la cantidad de
    palabras en $$A$$ de longitud $$r$$ es $$n^{r}$$.

## Subconjuntos

-   Cantidad de subconjuntos

    Un conjunto de $$n$$ elementos tiene exactamente $$2^{n}$$
    subconjuntos. 

-   Demostración

    Si $$X$$ tiene $$n$$ elementos, existe una biyección entre el
    conjunto de subconjuntos de $$X$$ y el conjunto de palabras de
    longitud $$n$$ en el alfabeto $$\{S,N\}$$.

# Permutaciones



-   Permutación

    Si $$A$$ es un alfabeto, una **permutación** de $$A$$ de longitud
    $$r$$ es una palabra de longitud $$r$$ que usa letras distintas.

-   Ejemplo

    Si $$A=\{x,y,z\}$$, las permutaciones de longitud 2 son:
    
    $$
    xy,xz,yx,yz,zx,zy.
    $$



-   Cantidad de permutaciones

    Si el alfabeto $$A$$ tiene $$n$$ elementos, la cantidad de
    permutaciones en $$A$$ de longitud $$r$$, donde $$r\leq n$$, es:
    
    $$
    n(n-1)(n-2)\cdots (n-r+1)=\frac{n!}{(n-r)!}.
    $$

-   

    En particular, si $$n=r$$, hay $$n!$$ permutaciones. Es decir,
    tiene sentido definir $$0!=1$$.

# Combinaciones



-   Combinación

    Si $$A$$ es un alfabeto con $$n$$ elementos, una **combinación** de
    tamaño $$r$$ de $$A$$ es un subconjunto de $$A$$ con $$r$$
    elementos.

-   Ejemplo

    Si $$A=\{x,y,z\}$$, las combinaciones de tamaño 2 son:
    
    $$
    \{x,y\},\{x,z\},\{y,z\}.
    $$



-   Cantidad de combinaciones

    Si el alfabeto $$A$$ tiene $$n$$ elementos, la cantidad de
    combinaciones en $$A$$ de longitud $$r$$, donde $$r\leq n$$, es:
    
    $$
    \frac{n!}{r!(n-r)!},
    $$
    
    esta cantidad se denota como $$\binom{n}{r}$$ y se llama un
    **coeficiente binomial**.

-   Corolario

    $$
    \binom{n}{r}=\binom{n}{n-r}
    $$

## Propiedades de los coeficientes binomiales

-   Teorema

    Si $$r<n$$ se tiene:
    
    $$
    \binom{n}{r}=\binom{n-1}{r-1}+\binom{n-1}{r}.
    $$

-   Demostración
    -   El lado izquierdo cuenta la cantidad de subconjuntos de tamaño $$r$$ de
        un conjunto $$X$$ de $$n$$ elementos.
    -   Sea $$x_{0}\in X$$ un elemento fijo, y dividimos a los
        subconjuntos de $$r$$ elementos de $$X$$ en dos clases: los que
        contienen a $$x_{0}$$ y los que no contienen a $$x_{0}$$.
    -   De los primeros hay $$\binom{n-1}{r-1}$$ y de los segundos
        hay $$\binom{n-1}{r}$$.

## El teorema del binomio

-   Teorema del binomio

    Para todo entero no negativo $$n$$ tenemos la igualdad de
    polinomios:
    
    $$
    (1+x)^{n}=\sum_{k=0}^{n}\binom{n}{k}x^{k}.
    $$

-   Corolario

    Para todo entero no negativo $$n$$ se tiene:
    
    $$
    2^{n}=\sum_{k=0}^{n}\binom{n}{k}.
    $$

## Ejercicios

-   Demuestra lo siguiente: (a) por medio de fórmula (b) por un
    argumento de conteo
    
    $$
    k\binom{n}{k}=n\binom{n-1}{k-1}.
    $$
-   Demuestra lo siguiente: (a) por medio de fórmula (b) por un
    argumento de conteo. Si $$0\leq c\leq b\leq a$$, se tiene que:
    
    $$
    \binom{a}{b}\binom{b}{c}=\binom{a}{a-c}\binom{a-c}{b-c}.
    $$



-   Sustituyendo $$x=-1$$ en el teorema del binomio, se demuestra que
    un conjunto $$A$$ tiene la misma cantidad de subconjuntos de
    tamaño par que subconjuntos de tamaño impar. Da una demostración
    combinatoria de tal hecho exhibiendo una biyección entre ambos
    conjuntos.
-   Derivando ambos lados respecto a $$x$$ en el teorema del binomio
    y sustituyendo $$x=1$$ se obtiene que:
    
    $$
    n2^{n-1}=\binom{n}{1}+2\binom{n}{2}+\cdots+n\binom{n}{n}.
    $$
    
    Encuentra una demostración combinatoria.
-   Si un entero $n$ tiene la factorización prima
    $$n=p_{1}^{r_1}p_{2}^{r_2}\cdots p_{k}^{r_k}$$ (es decir, los
    números $$p_{i}$$ son primos distintos y los $$r_{i}$$ son
    enteros positivos), ¿cuántos divisores tiene $$n$$?
