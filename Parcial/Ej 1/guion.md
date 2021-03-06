# Toma 1: Presentación de Ret


####### 1 ############
Hola, hoy trabajaremos sobre una teoría particular.
Sea 'tau ret' un tipo sin nombres de constantes, con nombres de funcion 'i' y 's', ambos de
aridad 2 y con un nombre de relación 'menor o igual' también de aridad 2.
Sea Ret la teoría de tipo 'tau ret' cuyo conjunto de axiomas es 'sigma Ret' , donde
sigma Ret es el siguiente conjunto de sentencias.

####### 2 ############
Notemos que tenemos axiomas que hablan sólo con respecto a la relación 'menor o
igual' y otros que hablan, también, de las funciones 's' e 'i'
$$$$ Esperar 4 segundos

####### 3 ############
Sobre esta teoría, daremos pruebas formales de las siguientes sentencias


####### 4 ############
$$$$$$$$$ Esperar 4 segundos


####### 5 ############

A partir de ahora, llamaremos FI a la primera sentencia y PSI a la segunda.
$$$$$$$$$ Esperar 6 segundos


# Toma 2

####### 7 ############

Comenzaremos estudiando un poco qué significa cada axioma de Ret.

Observemos primero que una estructura 'A' satisface los 3 primeros axiomas de 'ret' si y solo si el par
[A, menor o igual supra A] es un poset.


####### 8 ############

Otra observación importante es que una estructura A de tipo 'tau ret'  puede
satisfacer los 3 axiomas mencionados antes pero esto no implica que las
operaciones 'S supra A' e 'I supra A' deban ser las operaciones infimo y supremo
respecto al orden menor o igual supra A.

# Toma 3

####### 9 ############


Notar que una estructura A que satisfaga los 3 axiomas del orden satisfará el
axioma 'A s es C' si y solo si cualesquiera sean los elementos 'a', 'b' [la
interpretación de s en A, aplicada a 'a' y 'b'] es cota
superior del conjunto formado por a y b en el poset (A, menor o igual supra A).



####### 10 ############

Similarmente, una estructura A que satisfaga los 3 axiomas del orden cumplirá
'A s menor o igual C' si y solo si para todo 'a', 'b' [a s supra A b] es menor o
igual a toda cota superior del conjunto formado por a y b.


####### 11 ############

Osea que lo anteriormente visto dice que una estructura A cumplirá los 5 axiomas
mencionados si y sólo si, [menor o igual supra A] es un orden parcial y
la interpretación de s en A es la operación supremo respecto del orden
[menor o igual supra A]


# Toma 4
####### 12 ############

Razonando en forma similar obtenemos que una estructura A de tipo [tau ret]
satisface los axiomas de Ret, es decir es un modelo de Ret, si y solo si se
cumple la siguiente condición:

########  ##########
(A, menor o igual supra A) es un orden parcial


####### 13 ############
La interpretación de s en A es el supremo del poset


####### 14 ############
La interpretación de i en A es el infimo del poset


# Toma 5

####### 15 ############

A continuación mostraremos cómo encontrar una prueba formal en Ret de la
sentencia en pantalla.

$$$ ESPERAR 3 SEGUNDOS

Pero nosotros sabemos, por matemática básica, que en un modelo A de Ret la
operación [s supra A] es asociativa. Es decir, que todo modelo de Ret satisface
la sentencia a probar.


####### 16 ############

La forma que utilizaremos para encontrar la prueba formal será la siguiente:


###########
Primero, haremos una prueba matemática, imaginando que somos un matemático que
piensa en un modelo genérico de Ret y prueba en forma elemental, la sentencia
FI. Aquí por elemental entenderemos que sólo se podrá escribir sentencias de
tipo tau ret con posibles constantes extras y, además, lo único que se puede
usar son los axiomas de Ret y las típicas deducciones usadas en las pruebas
matemáticas.

 Además, siempre imaginaremos un modelo genérico de Ret, es decir no podremos
 usar nada de algún modelo particular concreto ya que queremos que la prueba
 obtenida sea válida para cualquier modelo de Ret.


####### 17 ############

Luego, usando la prueba matemática como guía, construiremos la prueba formal.


# Toma 6
####### 18 ############
Daremos entonces, primero, la prueba matemática de la sentencia FI.
Sea A un modelo fijo, pero arbitrario, de Ret
Sean a, b y c elementos de A fijos.


####### 19 ############
Probaremos que '(a s b) s c' es menor o igual que 'a s (b s c)'


####### 20 ############
Sabemos, por el axioma 'A s es cota' que
'a es menor o igual que 'a s (b s c)' ' y también que
'b s c es menor o igual que 'a s (b s c)''


####### 21 ############
Si aplicamos nuevamente el axioma, pero esta vez sobre 'b s c', sabemos que
'b es menor o igual que (b s c)' y que
'c es menor o igual que (b s c)'

####### 22 ############
Por dos y tres, y aplicando transitividad obtenemos
'b es menor o igual que 'a s (b s c)'


######  #######
 y por 2, 4 y transitividad obtenemos
'c es menor o igual que 'a s (b s c)'.

######  #######
Es decir que ahora hemos probado 7, 8 y 9



####### 23 ############
Pero por el axioma 'A 's' es menor o igual que toda cota', tomando
'x igual a "a"', 'ye igual a "b"' y 'z igual a ("a s (b s c)")'
tenemos que
'(a s b) es menor o igual que 'a s (b s c)' '


####### 24 ############
Y, finalmente, si aplicamos nuevamente el axioma, pero esta vez tomando
'x igual a (a s b)', 'y igual a c' y 'z igual a ('a' s (b s c))'

obtenemos que

''(a s b) s c' es menor o igual que 'a s (b s c)' '


####### 25 ############
Y así, como a, b y c eran elementos cualesquiera, probamos de manera matemática
que la sentencia FI se cumple en 'A'.


####### 26 ############

Ahora daremos la prueba formal en Ret de la sentencia en cuestión


######   ######

[VER EL TEMA DE SACAR LOS PARÉNTESIS]
Por axioma propio, sabemos que





----------------------------------------------------
########   #######
Ahora encontraremos una prueba formal en Ret de la sentencia Psi
Notese que Dis1 nos dice que se cumple la distributividad de i respecto del s.
Y la sentencia 'CansDobl' nos dice que en la estructura puede interpretarse
como una ley de cancelación doble en el sentido de que si x e y son elementos
para los cuales hay un z tal que se cumplen las igualdades [que corresponden,
agregarlas] entonces podemos cancelar tal 'z' y obtener la igualdad [x = y]


########   #######
Para ello, utilizaremos la misma metodología que usamos anteriormente:
Primero buscamos la prueba matemática y luego la formal.



########   #######
Usaremos el teorema auxiliar en pantalla, el cual llamaremos a partir de ahora
"teorema estrella".

Recomendamos que se realice la prueba del mismo como ejercicio.

probaremos un teorema auxiliar que utilizaremos más adelante.


########   #######
Ahora estamos en condiciones de probar la sentencia que queríamos.


########   #######
Primero supongamos que se cumple Dis1, es decir que
(para todo x), (para todo ye) y (para todo z) se da que
[(x i y) s (x i z)] es igual que [x i (y s z)]



########   #######
Probaremos, entonces, que se cumple CansDobl, es decir la propiedad en pantalla
[esperar 3 segundos]



########   #######
Sean a y b dos elementos de A fijos


########   #######
Probaremos, entonces, que se cumple la siguiente propiedad:
[esperar 4 segundos]


########   #######
Supongamos que se cumple el antecedente de la implicación, es decir la sentencia en pantalla.
[esperar 2seg]


########   #######
Supongamos 'c' es un elemento que cumple con la propiedad expresada en el antecedente.

Es decir:
[(a i c) es igual que (b i c)] y que [(a s c) es igual que (b s c)]


########   #######
Probemos entonces que ['a' es igual que 'b']



########   #######
Por teorema estrella, sabemos que

[(b s c) i b] es igual que 'b'

--------------------------------------------------------------

########   #######
Así, por el resultado (2) sabemos que [(a s c) es igual que (b s c)], por lo que

[(b s c) i b] es igual que [(a s c) i b]



########   #######
Y por la hipótesis mencionada en (1), tenemos que

[(a s c) i b] es igual que [(a i b) s (c i b)]


########   #######
Aplicando, nuevamente, el resultado 2 obtenemos que

[(a i b) s (c i b)] es igual que [(a i b) s (c i a)]


########   #######
Ahora, de nuevo por la hipótesis 1 y por conmutatividad de i (cuya prueba se deja
para el estudiante), sabemos  que

[(a i b) s (c i a)] es igual que [(b s c) i a]


########   #######
Y así, por 2

[(b s c) i a] es igual que [(a s c) i a]



########   #######
Finalmente, por el teorema estrella demostrado anteriormente,

[(a s c) i a] es igual que 'a'



########   #######
Pero esto quiere decir que
'a' es igual que 'b'



########   #######
Y así, hemos demostrado que, en Ret, se cumple la sentencia inicial que queriamos
probar.


########   #######
Ahora procederemos a dar la prueba formal en Ret de la sentencia en cuestión


########   #######
Para hacerla, utilizaremos los siguientes teoremas cuyas pruebas formales son dejadas
al lector
[esperar 3 segundos]


########   #######
[esperar 3 segundos]
