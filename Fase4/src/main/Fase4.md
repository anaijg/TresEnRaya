# ¡Primer movimiento!
## Descripción
¡Es hora de hacer que nuestro juego sea interactivo! Ahora vamos a añadir la capacidad para que el usuario haga un movimiento. Para esto, necesitamos dividir la cuadrícula en celdas. Supongamos que la celda superior izquierda tiene las coordenadas (1, 1) y la celda inferior derecha tiene las coordenadas (3, 3):

````scss
(1, 1) (1, 2) (1, 3)  
(2, 1) (2, 2) (2, 3)  
(3, 1) (3, 2) (3, 3)  
````
El programa debe pedir al usuario que introduzca las coordenadas de la celda donde quiere realizar su movimiento.

En esta etapa, el usuario jugará como X, no como O. Recuerda que la primera coordenada corresponde de arriba hacia abajo, y la segunda coordenada, de izquierda a derecha. Las coordenadas pueden incluir solo los números 1, 2 o 3.

¿Qué pasa si el usuario introduce coordenadas incorrectas? Podría introducir símbolos en lugar de números, elegir una celda ya ocupada o una celda fuera de la cuadrícula. Necesitas comprobar la entrada del usuario y manejar estas posibles excepciones.

### Objetivos
El programa debe funcionar de la siguiente manera:

1. Obtener la cuadrícula inicial 3x3 de la entrada como en las etapas anteriores. El usuario debe ingresar 9 símbolos que representen el campo, por ejemplo: _XXOO_OX_.
2. Mostrar esta cuadrícula 3x3 como en las etapas anteriores.
3. Pedir al usuario que realice un movimiento. Debe introducir dos números que representen las coordenadas de la celda donde quiere colocar su X, por ejemplo, 1 1.
4. Analizar la entrada del usuario. Si la entrada es incorrecta, informar al usuario del error:
    - Imprimir **This cell is occupied! Choose another one!** (¡Esta celda está ocupada! Elige otra) si la celda no está vacía.
    - Imprimir **You should enter numbers!** (¡Debes ingresar números!) si el usuario introduce símbolos no numéricos.
    - Imprimir **Coordinates should be from 1 to 3!** (¡Las coordenadas deben estar entre 1 y 3!) si el usuario introduce coordenadas fuera de la cuadrícula.
5. Seguir pidiendo al usuario que introduzca coordenadas hasta que la entrada sea válida.
6. Si la entrada es válida, actualizar la cuadrícula para incluir el movimiento del usuario e imprimir la cuadrícula actualizada en la consola.  

En resumen, debes mostrar el campo 2 veces: una vez antes del movimiento del usuario (basado en la primera línea de entrada) y otra vez después de que el usuario introduzca coordenadas válidas (momento en el que se actualiza la cuadrícula con el movimiento).

No elimines el código que escribiste en la etapa anterior. Lo necesitarás en la etapa final de este proyecto, así que puedes comentarlo si es necesario.

## Ejemplos
El símbolo de mayor seguido de un espacio (> ) representa la entrada del usuario. Nota que no forma parte de la entrada.
### Example 1:
````text
> X_X_O____
---------
| X   X |
|   O   |
|       |
---------
> 3 1
---------
| X   X |
|   O   |
| X     |
---------
````
### Example 2:
````text
> _XXOO_OX_
---------
|   X X |
| O O   |
| O X   |
---------
> 1 1
---------
| X X X |
| O O   |
| O X   |
---------
````
### Example 3:
````text
> _XXOO_OX_
---------
|   X X |
| O O   |
| O X   |
---------
> 3 3
---------
|   X X |
| O O   |
| O X X |
---------
````
### Example 4:
````text
> _XXOO_OX_
---------
|   X X |
| O O   |
| O X   |
---------
> 2 3
---------
|   X X |
| O O X |
| O X   |
---------
````
### Example 5:
````text
> _XXOO_OX_
---------
|   X X |
| O O   |
| O X   |
---------
> 3 1
This cell is occupied! Choose another one!
> 1 1
---------
| X X X |
| O O   |
| O X   |
---------
````
### Example 6:
````text
> _XXOO_OX_
---------
|   X X |
| O O   |
| O X   |
---------
> one
You should enter numbers!
> one one
You should enter numbers!
> 1 1
---------
| X X X |
| O O   |
| O X   |
---------
````
### Example 7:
````text
> _XXOO_OX_
---------
|   X X |
| O O   |
| O X   |
---------
> 4 1
Coordinates should be from 1 to 3!
> 1 4
Coordinates should be from 1 to 3!
> 1 1
---------
| X X X |
| O O   |
| O X   |
---------
````