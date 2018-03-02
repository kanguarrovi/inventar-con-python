# Escribiendo programas

![Matraz de Erlenmeyer](https://inventwithpython.com/invent4thed/images/00016.jpeg "Matraz de Erlenmeyer")

Ahora veremos lo que Python puede hacer con texto. Casi todos los programas
le muestran texto al usuario, y los usuarios le introducen texto a los 
programas a través del teclado. En este capítulo, harás tu primer programa,
el cual hace ambas cosas. Aprenderás a guardar texto en variables, combinar
texto, y mostrar el texto en la pantalla. El programa que crearás muestra el
saludo *Hello world* y pregunta por el nombre del usuario.

***
Temas cubiertos en este capítulo:
* String (hileras)
* Concatenación de strings
* Tipos de datos (como strings o enteros)
* Usar el editor de archivos IDLE para escribir programas
* Guardar y ejecutar programas en IDLE
* Flujo de ejecución
* Comentarios
* La función *print()*
* La función *input()*
* Sensibilidad de caso
***

## Valores *string*

En Python, los valores de texto son llamados *strings* (hileras en inglés).
Los strings pueden ser usadas como valores enteros o flotantes. Usted puede
guardar strings en variables. En el código, los strings empiezan y terminan
con comillas simples,'. Ingresa este cógido en la consola interactiva:

***
<pre>
>>> <b>spam = 'hello'</b>
</pre>
***

Las comillas simples le indican a Python donde el string comienza y donde
termina. Estas comillas no son parte del valor del texto del string. Ahora
si ingresas *spam* dentro de la consola interactiva, podrás ver el contenido
de la variable *spam*. Recuerda, Python evalua las variables como el valor
guardado dentro de la variable. En este caso, este es el string *hello*.

***
<pre>
>>> <b>spam = 'hello'</b>
>>> <b>spam</b>
'hello'
</pre>
***

Los strings pueden tener cuaquier caracter que posea el teclado dentro de
ellos y pueden ser tan largos como lo desees. Todos estos son ejemplos de
strings:

***
<pre>
'hello'
'Hi there!'
'KITTENS'
'7 apples, 14 oranges, 3 lemons'
'Anything not pertaining to elephants is irrelephant.'
'A long time ago, in a galaxy far, far away...'
'O*&#wY%*&OCfsdYO*&gfC%YO*&%3yc8r2'
</pre>
***

## Concatenación de strings

Usted puede combinar strings con operadores para crear expresiones, igual 
que como lo había hecho con los *ints* y *floats*. Cuando combinas dos 
strings con el operador de adición: '+', esa acción es llamada concatenación
de strings. Ejecuta 'Hello' + 'World!' en la consola interactiva:

***
<pre>
>>> <b>'Hello' + 'World!'</b>
'HelloWorld!'
</pre>
***

La expresión es evaluada como un único valor de tipo string: 'HelloWorld!'. 
No hay espacios entre las palabras porque no hay espacios en ninguno de los 
strings condatendos, a diferencia de este ejemplo:

***
<pre>
>>> <b>'Hello ' + 'World!'</b>
'Hello World!'
</pre>
***

El operador de adición ('+'), trabaja distinto con los valores de strings y 
los enteros porque son *tipos de datos* distintos. Todos los valores pretenecen
a un tipo de dato. El tipo de dato de 'Hello' es un string. El tipo de dato del 
valor 5 es un entero (int). El tipo de dato le dice a Python qué debe realizar
el operador cuando exalúa expresiones. El operador de adición concatena strings, 
pero suma valores enteros y flotantes.

## Escribiendo programas en el editor de archivos de IDLE

Hasta el momento, has estado escribiendo instrucciones dentro de la consola
interaractiva, una por una. Cuando escribes programas, ingresas varias 
intrucciones y son ejecutadas inmediatamente, y eso es lo que harás a 
continuación.¡Es hora de escribir tu primer programa!

Además del intérprete, el IDLE tiene otra parte llamada *file editor*
(editor de archivos). Para abrirlo, has click en la parte de *File* (Archivo)
del menu localizado en el pánel superior de la consola interactiva. Luego
selecciona *New file* (nuevo archivo). Una ventana en blanco aparecerá para
que escribar el código del programa dentro de ella, como se muestra en la
Figura 2-1.

![Editor de texto de IDLE](https://inventwithpython.com/invent4thed/images/00035.jpeg "Editor de texto de IDLE")

Figura 2-1: el editor de archivos (izquierda) y la consola interactiva (derecha)

Ambas ventanas parecen similares, pero recuerda: la consola interactiva tiene el 
prompt >>>, mientras que el editor de archivos no lo posee.

