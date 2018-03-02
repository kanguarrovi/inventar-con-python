# Escribiendo programas (Programando)/Escribiendo codigo

![Matraz de Erlenmeyer](https://inventwithpython.com/invent4thed/images/00016.jpeg "Matraz de Erlenmeyer")

Ahora veremos lo que Python puede hacer con texto.Casi todos los programas
le muestran texto al usuario, y los usuarios le introducen texto a los 
programas a través del teclado. En este capítulo, harás tu primer programa,
el cual hace ambas cosas. Aprenderás a guardar texto en variables, combinar
texto, y mostrar el texto en la pantalla. El programa que crearás muestra el
saludo 'Hola mundo' y pregunta por el nombre del usuario.

***
Temas cubiertos en este capítulo:
* String (cadenas)
* Concatenación de strings
* Tipos de datos (como strings o enteros)
* Usar el editor de archivos para escribir programas
* Guardar y ejecutar programas en IDLE
* Flujo de ejecución
* Comentarios
* La función 'print()'
* La función 'input()'
* Sensibilidad de caso
***

## Valores 'string'

En Python, los valores de texto son llamados 'strings' (cadenas en inglés).
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
si ingresas 'spam' dentro de la consola interactiva, podrás ver el contenido
de la variable 'spam'. Recuerda, Python evalua las variables como el valor
guardado dentro de la variable. En este caso, este es el string 'hello'.

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