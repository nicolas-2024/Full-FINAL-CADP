
* Informática: Es la ciencia que estudia el análisis y resolución de problemas utilizando computadoras.

* Memoria estática: La memoria estática es aquella donde se almacenan las variables de las cuales su tamaño no será alterado. Las variables solo cambian su contenido, no su tamaño.

* Memoria dinámica: La memoria dinámica es aquella donde las variables a almacenar no tienen un tamaño definido, y podrán aumentar o disminuir su tamaño tanto les sea permitido por la misma.

* Tipo de dato: El tipo de dato es un atributo, tanto para el ordenador, como para el programador, para saber qué valores manejará una variable declarada en memoria. Existen varios tipos de datos, y estos se dividen en simples y compuestos.

1. SIMPLES: Integer, real, boolean, char y puntero.
2. COMPUESTO: String y Estructuras (registro, lista y vector).
3. DEFINIDOS POR EL PROGRAMADOR.
*El tipo de dato real no admite div y mod.*

* Puntero:
  Un puntero es un tipo de dato simple que trabaja con la memoria dinámica.
Contiene la dirección de memoria en memoria dinámica donde se encuentra almacenado el dato real.
Este dato puede ser un entero, un real, un string y los demás tipos de datos, incluso otro puntero.


* Estructuras de control: If y else, case, while, for y repeat until.
If y Else: sentencia que modifica, o no, una sola vez la ejecución del programa.
	Estructura:
If (condición) then
		{pasos a realizar}
	else
		{pasos a realizar en caso contrario}

	Else es dependiente de If, no puede estar esta instrucción si anteriormente no hubo un if. 

* Case: Estructura de control que simula ser un if anidado, y analizará los diferentes casos dados, de esta forma realizará una acción dada al encontrar un caso verdadero.
Estructura:
case (condicion) of
	{instrucción 1}
{instrucción 2}
.
.
{instrucción n}

* While: estructura de control que se ejecuta en base a una condición, cero, una o n cantidad de veces realizando instrucciones. La condición debe ser finita, ya que podría producir un bucle infinito. La condición deberá ser verdadera para su correcto uso.
Estructura: 
while (condición) do
{paso a realizar}

* For: estructura de control que se ejecuta en base a una condición, una o n cantidad de veces. La condición de esta estructura tiende a ser finita, ya que se le da un valor de comienzo y uno de final.
	Estructura: 
	for (valor de comienzo) to (valor final) do
		{pasos a realizar}

* repeat until: estructura de control que se ejecuta antes de verificar la condición, una o más veces. El código se ejecuta tantas veces como la condición sea falsa. Se utiliza mayormente cuando quiere procesar el dato que cambia la condición a verdadera. Cabe recalcar, que la condición debe ser finita.
Estructura:
repeat
	{pasos a realizar}
until (condición)

**Diferencias entre if y case:**
If y case son lo mismo, simplemente, el case compara un dato con otros tantos, y en caso de cumplirse uno de estos, realizará una acción. En cambio, el if se utiliza para obtener una respuesta en base a un verdadero o falso, no obstante, se pueden anidar varios if y copiar la estructura de un case, pero esto hace menos legible al código.
En el case, al aceptar valores de tipo ordinal, se pueden especificar rangos dentro de las condiciones, en cambio, el if no tiene esta opción, y se debe realizar una condición que tape todas las posibilidades.

* Modularización: 
La modularización sirve para separar el código, de forma lógica, en diferentes partes, encapsulando código relacionado.
Ayuda a encontrar errores de forma más eficiente.
Hace más legible el código.
La reutilización es primordial cuando se habla de modularizar, evitamos programar el doble y reutilizamos el módulo en otra sección del código.

--- Procedure y Function:
En pascal existe el proceso y la función, que son dos formas de modularizar en un programa, estas están definidas por la siguiente sintaxis:

* Procedure nombreProceso (parámetros de E o E/S);
Características de procedure:
Podrá recibir datos, llamados parámetros por valor, y, eventualmente, podrá devolver datos, cuando el parámetro está definido por referencia.
Puede recibir, pero no necesariamente retornar un valor.
Puede no recibir ningún parámetro y funcionar igualmente.

* Function nombreFuncion (parámetros de entrada): tipoDeFuncion;
Características de function:
Podrá devolver un único valor, de tipo simple, definido en el encabezado de la función, luego de los parámetros.
Podrá recibir datos, pero no retornar los mismos.
Sus parámetros no pueden ser por referencia.
Para retornar un valor, se debe asignar un valor al nombre de la función, que es similar a una variable, guarda su valor en esa posición de memoria, de lo contrario, retornará basura.

* Caracteristicas de procedure y function:
Las variables definidas dentro de las mismas sólo serán exclusivas de estas, es decir, su alcance es local.
Se podrán llamar procesos y funciones dentro de las mismas.
Cuando se pasa un parámetro por valor, se realiza una copia de este dato, y podrá ser utilizada dentro del módulo sin alterar su valor original.
Los parámetros, al igual que las variables declaradas dentro del módulo, son locales al módulo.
Ambas pueden manipular variables globales.
Se pueden declarar types dentro de las mismas.

* Diferencias:
Procedure puede recibir parámetros de entrada, y también existe la opción de ser devueltos, function no tiene esta posibilidad, sólo podrá retornar un único valor.
Los tipos de datos devueltos por estos son diferentes en cada uno, mientras el procedure puede recibir y devolver cualquier tipo de dato, function solo puede devolver datos de tipo simple.

El tipo de dato que devolverá la función, al ser único, debe ser definido en el encabezado de la misma, y solo podrá devolver ese único tipo de dato, mientras que el proceso podrá devolver todos los tipos de datos que estén por referencia en la sección de parámetros


* Estructuras de datos: 
Permite al programador definir un tipo al que se asocian diferentes datos que tienen valores lógicamente relacionados y asociados bajo un nombre único.
Propiedades de las estructuras de datos:

Elementos: Homogenea y Heterogenea:
Homogénea: Los elementos que la componen son del mismo tipo.
Heterogénea: Los elementos que la componen pueden ser de distinto tipo.
Acceso: Secuencial y Directo.
Secuencial: Para ingresar a un valor, se debe tener un orden en particular.
Directo: Para ingresar a un valor, solo se debe saber dónde está posicionado, o cual es su identificador.
Linealidad: Lineal y no Lineal:
Lineal: Está formada por ninguno, uno o varios elementos que guardan una relación de adyacencia ordenada donde a cada elemento le sigue uno y le precede uno, solamente
No lineal: Para un elemento dado pueden existir 0, 1 ó más elementos que le suceden y 0, 1 ó más elementos que le preceden.
Tamaño: Dinamico y estatico:
Dinámico: El tamaño puede aumentar durante la ejecución del programa.
Estático: El tamaño no puede variar durante la ejecución del programa.


