# Conceptos básicos

## Notación

-   Inline math: \(x^2+y^2\). Display math:
    \[X^2+Y^2=\sin \theta\]

-   A menos que se indique, o que sea inmediato lo contrario, todos los
    conjuntos usados se suponen finitos, y las letras
    $m$, $n$, $r$, denotarán enteros positivos.

-   La cantidad de elementos del conjunto $X$ se denota con $\vert X\vert $.

-   El conjunto $\{1,2,\ldots,r\}$ se denotará como $[r]$.

-   En varios problemas, se describen un conjunto $X$, un subconjunto
    $Y\subseteq X$ y se plantea el problema de determinar $\vert Y\vert $.

-   En otros problemas más avanzados, se describe una familia de
    subconjuntos $$Y_{n}\subseteq X$$, y se busca determinar la
    función $$f(n)=\vert Y_{n}\vert $$.

## Reglas de la suma y del producto

-   Regla de la suma

    Si los conjuntos $A$, $B$ son tales que $A\cap B=\emptyset$,
    entonces:
    
    $$
    |A\cup B|=|A|+|B|.
    $$

-   Regla del producto

    Para cualesquiera conjuntos finitos $$A,B$$, se tiene que:
    
    $$
    |A\times B| = |A||B|
    $$

## Problema

-   Problema

    Una contraseña consta de 8 caracteres. Cada carácter puede ser uno
    de 26 letras, o bien uno de 10 dígitos. También se pide que la
    contraseña debe tener al menos un dígito. ¿Cuántas contraseñas
    válidas son posibles? (Por ejemplo, `abcdefgh` no es válida pero
    `abcdefg5` sí).



-   Solución
    -   El problema equivale a formar &ldquo;palabras&rdquo; de longitud 8 con 36
        &ldquo;símbolos&rdquo; diferentes, pero con la condición de que uno de `0`, `1`,
        `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`, debe estar presente.
    -   Si no hubiera la condición de que debe haber un dígito, la
        respuesta sería $$36^{8}$$.
    -   Como hay $$26^{8}$$ contraseñas que usan solo letras hay
        $$36^{8}-26^{8}$$ contraseñas que no usan solo letras, es decir,
        en donde aparece un dígito.

# Problemas



-   Si se tiene tela de 5 colores distintos, ¿de cuántas maneras se
    puede hacer una bandera con franjas de tres colores?
    (suponiendo, primero que los colores se pueden repetir y luego
    que no). Repetir las preguntas suponiendo que el rojo tiene que
    ser uno de los colores escogidos.
-   ¿En cuántas de las $6!$ \`\`palabras&rsquo;&rsquo; de 6 letras distintas que se
    pueden formar con las letras ABCDEF se tiene que la A aparece
    junto a la D?
-   ¿Cuántos números enteros entre 1000 y 9999 no tienen al 9 como
    uno de sus dígitos?
-   ¿Cuántos números enteros entre 1000 y 9999 no tienen dígitos
    repetidos?
-   ¿De cuántas maneras se pueden escoger dos libros de diferentes
    materias de entre 5 libros de álgebra, 4 de análisis y 6 de variable
    compleja?
