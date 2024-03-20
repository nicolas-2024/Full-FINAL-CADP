
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

1. Elementos: Homogenea y Heterogenea:
2. Homogénea: Los elementos que la componen son del mismo tipo.
3. Heterogénea: Los elementos que la componen pueden ser de distinto tipo.
4. Acceso: Secuencial y Directo.
5. Secuencial: Para ingresar a un valor, se debe tener un orden en particular.
6. Directo: Para ingresar a un valor, solo se debe saber dónde está posicionado, o cual es su identificador.
7. Linealidad: Lineal y no Lineal:
8. Lineal: Está formada por ninguno, uno o varios elementos que guardan una relación de adyacencia ordenada donde a cada elemento le sigue uno y le precede uno solamente
9. No lineal: Para un elemento dado pueden existir 0, 1 ó más elementos que le suceden y 0, 1 ó más elementos que le preceden.
10. Tamaño: Dinamico y estatico:
11. Dinámico: El tamaño puede aumentar durante la ejecución del programa.
12. Estático: El tamaño no puede variar durante la ejecución del programa.

*Registros* : Un registro es una estructura de datos que contiene elementos en su interior, comúnmente llamados campos, donde cada uno tiene un identificador y un tipo de dato. Estos datos siempre están relacionados, ya que provienen de los atributos de algo en particular. El registro es directo, ya que para ingresar a cada posición se debe saber el identificador del campo, y heterogénea, ya que sus elementos pueden ser de diferentes tipos, como también, pueden ser todos de un mismo. Es estático.

*Vector* : Un vector es una estructura de datos que contiene casillas, de las cuales, cada una contiene un dato, y cada casilla tiene un número que la identifica dentro del vector que va desde 1 hasta el ingresado por el programador, conocida como dimensión física. Es directo, porque se puede ingresar a cualquier casilla sin necesidad de haber recorrido las anteriores. Es homogénea, ya que, el vector solo admite en sus casillas elementos del mismo tipo. Es de tamaño estático, ya que su tamaño será el declarado, y una vez compilado no podrá aumentarse.

*Listas* : Una lista, es una estructura de datos dinámica, que trabaja con punteros y nodos. Un puntero y nodo inicial comienza la lista, y contendrá, en alguno de sus campos, la siguiente posición de memoria donde se encuentre el próximo nodo para continuar la lista. Una lista es de acceso secuencial, ya que para llegar al último nodo, se deberá recorrer cada uno, hasta encontrar uno que, en el campo del siguiente nodo contenga “nil”. Es de tamaño dinámico, ya que su tamaño irá aumentando o disminuyendo a medida que se ejecute el programa, utilizando las instrucciones correspondientes (new o dispose).

*Algoritmos de búsqueda** : Un algoritmo de búsqueda es un conjunto de instrucciones que están diseñadas para localizar un elemento con ciertas propiedades dentro de una estructura de datos.

*Búsqueda secuencial:*  se basa en buscar un elemento dentro de un vector, de principio a fin, o hasta ser encontrado. En caso de que este desordenado, este será el más “eficiente”, en caso de que este ordenado, será ineficiente.

* Código en GitHub:* 
https://github.com/NicaOB/Algoritmos-de-busqueda/blob/main/busquedaSecuencial.pas

A partir del siguiente algoritmo, debe estar ordenado por medio del elemento que se desee buscar.
Búsqueda secuencial en vector ordenado: Se procede a condicionar la búsqueda dentro del algoritmo, dejando un límite de búsqueda.

Código en GitHub:
https://github.com/NicaOB/Algoritmos-de-busqueda/blob/main/BusquedaSecuencialOrdenada.pas

* Búsqueda binaria o dicotómica: Este algoritmo, a diferencia de los anteriores, comienza su búsqueda por la mitad del vector, comparando el elemento buscado con esta posición, y en caso de no ser el elemento a buscar, el algoritmo decidirá ir a la primera mitad o a la segunda mitad. Este proceso se repetirá n cantidad de veces, hasta que se encuentre o no el elemento

Algoritmos de eliminación: Un algoritmo de eliminación se basa en buscar un elemento en una estructura de datos adecuada, y eliminar el dato.

Eliminación en vector: Para eliminar un elemento de un vector, se debe tener en consideración las siguientes cuestiones:
La posición que se pida este dentro del rango de la dimensión lógica.
Realizar el corrimiento desde la posición deseada, hasta el final.
Decrementar en uno la dimensión lógica.

*Eliminación en lista: Eliminar un elemento de una lista, implica recorrer la lista, hasta encontrar el elemento deseado y eliminarlo con dispose.*

* Corrección y eficiencia: Cuando se habla de corrección y eficiencia se habla en base a un algoritmo. Y se divide en dos, corrección y eficiencia del mismo:

**Corrección:** proceso que da a conocer los posibles errores que pueda tener un algoritmo, y consta de 4 etapas, no necesariamente conectadas:
*Testing:* Se diseña un plan de pruebas, para comprobar que el algoritmo realiza lo solicitado. Para realizar un plan de pruebas correcto se tiene en cuenta lo siguiente: 
Saber que se debe testear y buscar datos de prueba para esos segmentos.
 Determinar el resultado que se espera en cada prueba. 
Poner atención en los casos límites.
Diseñar los casos de prueba e implementarlos al programa.
Debugging: Se basa en escribir sentencias en diferentes partes del código, que estén relacionadas con el error a encontrar, para ver dónde se encuentra el problema, y solucionarlo posteriormente.
*Error sintáctico:* se muestra en la compilación del programa.
*Error lógico:* se muestra en la ejecución del programa.
*Error del sistema:* son pocos comunes.
**Walkthrough:** Recorrer un programa frente a personas, de forma que, se pueda encontrar un error rápidamente, con ayuda de la audiencia.
Verificación: Significa controlar que se cumplan las pre y post condiciones del mismo.
**Eficiencia:** Una vez el programa es correcto, sigue ver la eficiencia de los algoritmos, analizando el tiempo que tarda el algoritmo en ejecutarse, y la memoria que requiere.
Esta palabra se relaciona con:
1. Datos de entrada (tamaño y cantidad).
2. Calidad del código generado por el compilador.
3. Naturaleza y rapidez en la ejecución de las instrucciones de máquina.
4. El tiempo del algoritmo base.

La eficiencia va ligada al tiempo de ejecución, que en pocas palabras, es el tiempo que tarda el algoritmo en finalizar. Este se mide de dos maneras, de forma empírica o teórica:
Empírica: se ejecuta en un ordenador y se analiza el tiempo de comienzo y final del algoritmo, pero se debe tener en cuenta que cada ordenador es diferente, por ende, el tiempo de ejecución está ligado a este factor, también, depende de los datos que se ingresen.
Teórica: se busca realizar una medida en UT (unidad de tiempo) de forma general, en cada instrucción. De esta forma, se obtiene un valor más exacto en tiempo de ejecución, que será igual para todas los ordenadores, aunque sigue variando en sus componentes, este valor en UT es una medida que se respetará en todos por igual. Todas las instrucciones elementales miden una unidad de tiempo, es decir 1 UT.

**Medición de memoria:**
    La medición de memoria de un programa consta de dos partes, la memoria estática, y la memoria dinámica. La memoria estática es aquella que su espacio va a ser al declarado al inicio, y compilado el programa, y esta no variará durante la ejecución del mismo. Mientras que la memoria dinámica no respeta un espacio exacto, sino que, crecerá tanto el programador lo pida, o el sistema operativo lo permita, aclarando que esta se verá modificada durante la ejecución del programa.

char
1 byte
boolean
1 byte
integer
4 bytes
real
8 bytes
string
tamaño + 1 byte
subrango
depende el tipo
registro
suma de los campos
arreglos
dim. Fisica * tipo de dato
puntero
4 bytes (en mem. estática)

