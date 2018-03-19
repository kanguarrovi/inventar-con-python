# Escribiendo programas

![Matraz de Erlenmeyer](https://inventwithpython.com/invent4thed/images/00016.jpeg "Matraz de Erlenmeyer")

<p align="justify">
Ahora veremos lo que Python puede hacer con texto. Casi todos los programas
le muestran texto al usuario, y los usuarios le introducen texto a los 
programas a través del teclado. En este capítulo, harás tu primer programa,
el cual hace ambas cosas. Aprenderás a guardar texto en variables, combinar
texto, y mostrar el texto en la pantalla. El programa que crearás muestra el
saludo *Hello world* y pregunta por el nombre del usuario.
</p>

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
con comillas simples (''). Ingresa este códido en la consola interactiva:

***
<pre>
>>> <b>spam = 'hello'</b>
</pre>
***

<p align="justify">
Las comillas simples le indican a Python donde el string comienza y donde
termina. Estas comillas no son parte del valor del texto del string. Ahora
si ingresas *spam* dentro de la consola interactiva, podrás ver el contenido
de la variable *spam*. Recuerda, Python evalua las variables como el valor
guardado dentro de la variable. En este caso, este es el string *hello*.
</p>

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

## Creando el programa *Hello World!*

Es una tradicción para los programadores que el primer programa que realicen
muestre *Hello world!* en la pantalla. Ahora mismo crearás tu primer programa
*Hello World!*.

![Usando Python 3 en vez de Python 2](https://inventwithpython.com/invent4thed/images/00038.jpeg "Usando Python 3 en vez de Python 2")

Cuando escribas tu programa, recuerda no incluir los numberos al principio de
cada línea de código. Estos números están incluídos en este libro para poder
referenciar la línea donde se encuentra el código. La esquina inferior derecha
del editor de archivos te indicará donde se encuentra el cursor, de esta manera
podrás verificar en cual línea de código te encuentras. La figura 2-2 muestra
que el cursor está en la línea 1 (de arriba hacia abajo del editor) y la
columna 0 (de izquierda a derecha).

![Posicionamiento del cursor](https://inventwithpython.com/invent4thed/images/00039.jpeg "Posicionamiento del cursor")

Figura 2-2: La esquina inferior derecha del editor de archivos te dice donde
se encuentra el cursor.

Ingresa el siguiente texto dentro de la nueva ventana del editor de archivos.
Este es el *código fuente* del programa. Contiene las instrucciones que Python
va a seguir cuando el programa sea ejecutado.

*hello.py*

***
<pre>
1. # This program says hello and asks for my name.
2. print('Hello world!')
3. print('What is your name?')
4. myName = input()
5. print('It is good to meet you, ' + myName)
</pre>
***

IDLE marcará las diferentes instrucciones con colores distintos. Después de que
hayas escrito el código, la ventana deberá verse como la Figura 2-3.

![Ventana IDLE](https://inventwithpython.com/invent4thed/images/00041.jpeg "Ventana IDLE")

Figura 2-3: el editor de archivos se verá como esto cuando hayas escrito el código.

Verifica si tu ventana de IDLE se ve parecida.

## Guardando tu programa

Cuando hayas entrado a tu código fuente, guárdalo haciendo click en
File -> Save As. (Archivo -> Guardar como). O presionando Ctrl + S para
guardarlo con el atajo del teclado. La Figura 2-4 muestra la ventana de
*Guardar como* cuando es abierta. Nombra el archivo como *hello.py* en
área de texto y luego has click en Save (Guardar).

![Ventana de guardado](https://inventwithpython.com/invent4thed/images/00043.jpeg "Ventana de guardado")

Figura 2-4: Guardando tu programa.

Recurrentemente deberías guardar tus programas mientras los escribes.
De esa manera, si el ordenador falla o te sales accidentalmente del IDLE,
no perderás mucho trabajo que hayas realizado.

Para cargar tu programa previamente guardado, has click en File -> Open 
(Archivo -> Abrir). Selecciona el archivo *hello.py* en la ventana que 
aparece y has click sobre el botón Open (Abrir). Tu programa *hello.py*
será abierto en el editor de archivos.

## Ejecutando tu programa

Es hora de ejecutar el programa. Has click en Run->Run Module. O sólo presiona F5 desde el editor de archivos (FN-5 en Mac). Tu programa será
ejecutado desde la consola interactiva.

Ingresa tu nombre cuando el programa te lo solicite. Se parecerá como
la Figura 2-5.

![Consola interactiva despues de ejecutar hello.py](https://inventwithpython.com/invent4thed/images/00045.jpeg "Consola interactiva despues de ejecutar hello.py")

Figura 2-5: Consola interactiva despues de ejecutar hello.py

Cuando ingresas tu nombre y presionas ENTER, el programa te saludará por
tu nombre. ¡Felicidades! Has escrito tu primer programa y ahora eres un(a)
programador(a). Presiona F5 de nuevo para ejecutar el programa una segunda
vez e ingresar un nombre distinto.

Si tienes algún error, compara tu código con el código de este libro en
la [Herramienta Diff](https://nostarch.com/inventwithpython#diff)
(En idioma inglés) Copia y pega tu código desde el editor de archivos a
la página web y haz click en el botón que dice <b>Compare</b>. Esta 
herramienta destacará cualquier diferencia que haya entre tu código y
el código en este libro, como se muestra en la Figura 2-6.

Mientras programas, si tienes un <b>NameError</b> que se ve como el de
a continuación, eso significa que estás utilizando Python2 en lugar de
Python3.

***
<pre>
Hello world!
What is your name?
<b>Albert</b>
Traceback (most recent call last):
  File "C:/Python26/test1.py", line 4, in <module>
    myName = input()
  File "<string>", line 1, in <module>
NameError: name 'Albert' is not defined
</pre>
***

Para solucionar este problema, install Python3.4 y vuelve a ejecutar el
programa. (Ve a "Descargar e instalar Python" en la página xxv.)

![Herramienta Diff](https://inventwithpython.com/invent4thed/images/00048.jpeg "Herramienta Diff")

Figura 2-6: Usando la herramienta Diff en https://www.nostarch.com/inventwithpython#diff

## Como funciona el programa *Hello World*

Cada línea de código es una instracción interpretada por Python. Estas
instrucciones crean el programa. Las instrtaciones de un programa de 
computadora son como pasos en una receta. Python ejecuta cada
instruccion en orden, comenzando desde la cima del programa
moviendose hasta abajo.

El paso por el que Python está actualmente trabajando en el programa
se llama la *ejecución*. Cuando un programa comienza, la ejecución is
la primera instrucción. Después de ejecutada la instrucción, Python
va hacia la siguiente instrucción.

Veamos cada línea de código para observar qué está haciendo. Comenzaremos
en la línea número 1.

## Comentarios para el programador
La primera línea del programa *Hello World* es un comentario.

***
<pre>
1. # This program says hello and asks for my name.
</pre>
***

Todo texto seguido de la marca numeral (#) es un comentario. Los
comentarios son las notas informativas acerca de lo que el código hace;
no están escritas para Python, sino para ti, el programador. Python ignora
los comentarios cuando ejecuta un programa. Los programadores usualmente
ponen un comentario el la parte de arriba del código para ponerle un
título a su programa. El comentario en el programa *Hello World* te dice
que el programa saluda y pregunta por tu nombre.

## Funciones: miniprogramas dentro de programas

Una función es como un miniprograma dentro de tu programa que contiene 
algunas instrucciones para ejecutar en Python. Lo genial acerca de las
funciones es que sólo necesitas saber qué es lo que hacen, y no como lo
hacen. Python provee algunas funciones implementadas. Usamos *print()* e
*input()* en el programa *Hello World*.

Una funcion de *llamada* es una instrucción que le dice a Python que
ejecute el código dentro de una función. Por ejemplo, tu programa llama
la función *print()* para mostrar un string en la pantalla. La función
*print()* toma el string que escribiste dentro de los paréntesis como
un argumento de entrada y lo muestra en la pantalla.

## La función *print()*

Las líneas 2 y 3 del programa *Hello World* son llamadas a *print()*:

***
<pre>
2. print('Hello world!')
3. print('What is your name?')
</pre>
***

Un valor entre paréntesis en la función es llamado como *argumento*. El
argumento de la llamada *print()* en la línea 2 is 'Hello world!', y 
el argumento de la llamada *print()* en la línea 3 es 'What's your name?'.
Esto es llamado como *pasar* el argumento a la función.

##La función *input()*

La línea 4 es una declaración de asignación de una variable, *myName*,
y una función de llamada, *input()*:

***
<pre>
4. myName = input()
</pre>
***

Cuando *input()* es llamada, el programa espera para que el usuario 
ingrese un texto. El string de texto que el usuario ingresa se convierte
en el valor que la llamada a función evalúa. Las llamadas a función
pueden ser usadas dentro de expresiones en cualquier lugar donde un valor
pueda ser usado.

El valor que la llamada a función se llama valor de retorno (return value).
(De hecho, "el valor que la llamada de una función retorna" significa lo 
mismo que "el valor que la llamada a función evalúa".) En este caso, el 
valor de retorno de la función *input()* es el string que el usuario
ingresó: su nombre. Si el usaurio ingresa *Albert*, la llamada 
función *input()* evalúa el string 'Albert'. La evaluación se ve como esto:

![Evaluación de funcion](https://inventwithpython.com/invent4thed/images/00049.jpeg "Evaluacion de funcion")

##Expresiones en llamadas a funciones

La última línea de código en el programa *Hello World* es otra llamada a
la función *print()*:

***
<pre>
5. print('It is good to meet you, ' + myName)
</pre>
***

La expresión *'It is good to meet you', + myName* está rodeada por los 
paréntesis del *print()*. Porque los argumentos son valores únicos, Python
evaluará primero esta expresión y luego pasará ese valor como el argumento.
Si myValue contiene el valor 'Albert', la evaluación se verá así:

![Evaluación de Albert](https://inventwithpython.com/invent4thed/images/00051.jpeg "Evaluacion de Albert")
Así es como el programa saluda al usuario por su nombre.

##El final del programa
Una vez el programa executa la última línea, *termina* o *sale*. Esto
significa que el programa para de ejecutarse. Python olvida todos los
valores de las variables, incluído el string guardado en *myName*. Si
ejecutas el programa otra vez e ingrasas un nombre diferente, el
programa pensará que es tu nombre:

***
<pre>
Hello world!
What is your name?
Carolyn
It is good to meet you, Carolyn
</pre>
***

Recuerda, la computadora hace exactamente lo que la programaste para hacer.
Las computadoras son tontas y sólo siguen las instrucciones que les diste
de forma exacta. La computadora no le importa si le ingresas tu nombre, o
el nombre de otra persona o algo sin sentido. Escribe e ingresa lo que quieras. La computadora lo tratará de la misma manera:

<pre>
Hello world!
What is your name?
<b>shoe</b>
It is good to meet you, shoe.
</pre>
***