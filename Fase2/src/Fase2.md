# El usuario es el maestro del juego
## Descripción
Nuestro programa debe ser capaz de mostrar la cuadrícula en todas las etapas del juego. Ahora vamos a escribir un programa que permita al usuario introducir una cadena que represente el estado del juego y que imprima correctamente la cuadrícula 3x3 en función de esa entrada. También añadiremos algunos bordes alrededor de la cuadrícula del juego.

## Objetivos
En esta etapa, escribirás un programa que:

1. Lea una cadena de 9 símbolos desde la entrada y la muestre al usuario en una cuadrícula 3x3. La cuadrícula solo puede contener los símbolos X, O y _.
2. Imprima una línea de guiones (---------) por encima y por debajo de la cuadrícula, añada el símbolo de barra vertical (|) al inicio y al final de cada línea de la cuadrícula, y añada un espacio entre todos los caracteres de la cuadrícula.
## Ejemplos
El símbolo de mayor seguido de un espacio (> ) representa la entrada del usuario. Nota que no forma parte de la entrada.

### Ejemplo 1:
````text
> O_OXXO_XX
---------  
| O _ O |  
| X X O |  
| _ X X |
--------- 
````

### Ejemplo 2:
````text
> OXO__X_OX  
---------  
| O X O |  
| _ _ X |  
| _ O X |  
---------  
````

### Ejemplo 3:
````text
> _XO__X___  
---------  
| _ X O |  
| _ _ X |  
| _ _ _ |  
---------  
````