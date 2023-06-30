# Moda media y mediana
La tarea consistió en desarrollar una aplicación en lenguaje ensamblador que calcule la moda, mediana y la media  para un conjunto de datos ingresados por el usuario.
Primeramente el programa te pide introducir una lista ordenada de números por lo que el usuario debe introducir el primer número presionar ENTER, introducir el segundo y presionar ENTER y así consecutivamente hasta completar la lista la cual tiene un tamaño de 7 números en total. Luego de realizar lo anteriormente descrito se muestran los resultados de la mediana, la media y la moda para luego mostrarle un cartel al usuario HASTA LUEGO, GRACIAS POR TODO.

El programa contiene tres segmentos:

 Segmento de datos: que es el almacén de las variables utilizadas
 Segmento de pila: donde se declara la capacidad de la pila(DB 64 DUP(?))
 Segmento de codigo: donde  va todo el código del programa y a continuación mencionaré lo desarrollado en este

Para insertar los números de la lista utilice etiquetas como MOV, también utilice una macro llamada SCAN_NUM que proviene de una biblioteca importada llamada emu 8086 ,al insertar los elementos de la lista comencé el proceso. Primeramente hallar la media, para esto creé una etiqueta llamada SUMA 1 en la cual se va sumando cada valor de cada posición de la lista y se almacenan en la variable MEDIA, luego salta una etiqueta llamada PROMEDIO la cual divide la cantidad de elementos que tiene entre 7 devolviendo el valor de la media y se imprime por pantalla con una macro llamada PRINT_NUM_UNS. Despues la mediana (esta no es más que el elemento que se encuentra en el medio de la lista) y como esta ya estaba ordenada se realizó un método que devuelve el elemento que esta en la posición número 3 que es la del medio. Para finalmente hallar la moda en la cual utilice dos registros contadores uno llamado CONTADOR y el otro CONTADOR MÁX que van recorriendo la lista y comparando para saber cual es el número que más se repite (algoritmo muy conocido) para así poder cumplir con el objetivo del trabajo 

A medida que iba avanzando en el desarrollo de la aplicación me enfrenté a desafios y obstáculos tpicos de la programación en lenguaje ensamblador, como la gestión de registros, el manejo de bucles y la optimización del código para mejorar la eficiencia 
Para abrir el programa abra el ejecutable en el emu8086 y presione RUN 
 

 Trabajo final en ensamblador
