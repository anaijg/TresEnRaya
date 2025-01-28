# ¡Lucha!
## Descripción
¡Nuestro juego está casi listo! Ahora combinemos lo que hemos aprendido en las etapas anteriores para crear un juego de tres en raya (tic-tac-toe) que dos jugadores puedan jugar desde el principio (con una cuadrícula vacía) hasta el final (cuando haya un empate o uno de los jugadores gane).

El primer jugador jugará como X, y su oponente jugará como O.

## Objetivos
En esta etapa, debes escribir un programa que:

1. Imprima una cuadrícula vacía al comienzo del juego.
2. Cree un bucle de juego donde el programa pida al usuario que introduzca las coordenadas de la celda, analice si el movimiento es correcto y muestre la cuadrícula con los cambios si todo está bien.
3. Termine el juego cuando alguien gane o haya un empate.
4. Muestre el resultado final al final del juego. ¡Buena suerte!
## Ejemplos
El símbolo mayor seguido de un espacio (> ) representa la entrada del usuario. Nota que no forma parte de la entrada.
### Ejemplo 1.
````scss
---------
|       |
|       |
|       |
---------
> 2 2
---------
|       |
|   X   |
|       |
---------
> 2 2
This cell is occupied! Choose another one!
> two two
You should enter numbers!
> 1 4
Coordinates should be from 1 to 3!
> 1 1
---------
| O     |
|   X   |
|       |
---------
> 3 3
---------
| O     |
|   X   |
|     X |
---------
> 2 1
---------
| O     |
| O X   |
|     X |
---------
> 3 1
---------
| O     |
| O X   |
| X   X |
---------
> 2 3
---------
| O     |
| O X O |
| X   X |
---------
> 3 2
---------
| O     |
| O X O |
| X X X |
---------
X wins
````