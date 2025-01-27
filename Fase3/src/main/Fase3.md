# ¿Qué pasa en el campo?
## Descripción
En esta etapa, vamos a analizar el estado del juego para determinar si alguno de los jugadores ya ha ganado, si el juego aún está en curso, si ha terminado en empate, o si el usuario ha introducido un estado de juego imposible (dos ganadores, o un jugador que ha hecho demasiados movimientos).

## Objetivos
En esta etapa, tu programa debe:

1. Tomar una cadena introducida por el usuario e imprimir la cuadrícula del juego como en la etapa anterior.
2. Analizar el estado del juego y mostrar el resultado. Los posibles estados son:  

    - **Game not finished (Juego no terminado)**: cuando ningún jugador tiene tres en línea y aún hay celdas vacías.

    - **Draw (Empate)**: cuando ningún jugador tiene tres en línea y no hay celdas vacías.  

    - **X wins (X gana)**: cuando la cuadrícula tiene tres X en línea (incluyendo diagonales).  

    - **O wins (O gana)**: cuando la cuadrícula tiene tres O en línea (incluyendo diagonales).  

    - **Impossible (Imposible)**: cuando la cuadrícula tiene tres X en línea y también tres O en línea, o cuando hay muchas más X que O (o viceversa). La diferencia de movimientos debe ser 1 o 0; si es 2 o más, el estado es imposible.

En esta etapa, asumiremos que tanto X como O pueden iniciar el juego.

Puedes elegir usar un espacio o un guion bajo (_) para imprimir las celdas vacías.

## Ejemplos
El símbolo de mayor seguido de un espacio (> ) representa la entrada del usuario. Nota que no forma parte de la entrada.

### Ejemplo 1:
````text
> XXXOO__O_  
---------  
| X X X |  
| O O _ |  
| _ O _ |  
---------  
X wins  
````

### Ejemplo 2: 
````text
> XOXOXOXXO  
---------  
| X O X |  
| O X O |  
| X X O |  
---------  
X wins  
````

### Ejemplo 3: 
````text
> XOOOXOXXO  
---------  
| X O O |  
| O X O |  
| X X O |  
---------  
O wins  
````

### Ejemplo 4: 
````text
> XOXOOXXXO  
---------  
| X O X |  
| O O X |  
| X X O |  
---------  
Draw  
````

### Ejemplo 5: 
````text
> XOXOOXXXO  
---------  
| X O X |  
| O O X |  
| X X O |  
---------  
Draw  
````

### Ejemplo 6: 
````text
> XO_XO_XOX  
---------  
| X O _ |  
| X O _ |  
| X O X |  
---------  
Impossible  
````

### Ejemplo 7
````text
> _O_X__X_X  
---------  
|   O   |  
| X     |  
| X   X |  
---------  
Impossible  
````

### Ejemplo 8: 
````text
> _OOOO_X_X  
---------  
|   O O |  
| O O   |  
| X   X |  
---------  
Impossible  
````

