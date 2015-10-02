# investigacion

VARIABLE ESTATICA
Es una variable que ha sido ubicada estáticamente y cuyo tiempo de vida se extiende durante toda la ejecución del programa. Normalmente una variable estática tiene un ámbito más amplio que otras variables. Los valores de variables estáticas se pueden establecer una vez (durante el tiempo de ejecución) o se pueden cambiar en múltiples ocasiones durante la ejecución del programa. La terminología "variable estática" se basa en C y C++, pero también se usa en muchos lenguajes de programación derivados. En lenguajes de diferente origen el mismo concepto puede denominarse "variable global".

En el lenguaje de programación C se usa static con variables globales y funciones para restringir su ámbito al archivo donde se definen. Con variables locales, static se usa para almacenar la variable en la memoria asignada de forma estática en lugar de en la memoria asignada de forma automática. Siempre y cuando el lenguaje no fije la implementación del tipo de memoria a usar, la memoria asignada de forma estática se reserva normalmente en el segmento de datos del programa durante la compilación, mientras que la memoria asignada de forma automática es normalmente implementada como pila de llamadas transitorio.

CICLO DE VIDA DE LAS VARIABLES
• Variables de instancia (u objeto):
Se crean cuando se crea el objeto que las contiene. Se inicializan por defecto si no se hace de modo explícito; 0 para números, "false" para booleano, "null" para objetos y se destruyen cuando el recolector de basura de Java no encuentra referencias activas para el objeto. 
• Variables estáticas (o de clase): 
Se crean cuando la clase se usa por primera vez. Se inicializan por defecto si no se hace de modo explícito; 0 para números, "false" para booleano, "null" para objetos y suelen existir para el resto del programa (salvo que no esté cargado). 
• Variables locales (o de bloque): 
Creadas en la sentencia en la que están definidas. No se inicializan por defecto. Contienen datos imprevisibles y se destruyen al salir del bloque (en la llave final).

Comprensión del ciclo de vida de las variables

El tiempo durante el que una variable conserva su valor se denomina duración. El valor de una variable puede cambiar durante su duración, pero conservará algún valor. Cuando una variable pierde ámbito, ya no tiene un valor.
Cuando un procedimiento comienza a ejecutarse, se inicializan todas las variables. Una variable numérica se inicializa en cero, una cadena de longitud variable se inicializa en una cadena de longitud cero ("") y una cadena de longitud fija se completa con el carácter representado por el código de carácter ASCII 

Cuando declara una variable de objeto, se reserva espacio en la memoria, pero el valor se establece en Nothing hasta que asigne una referencia de objeto a ella con la instrucción Set.
Si el valor de una variable no ha cambiado durante la ejecución del código, conserva el valor inicializado hasta que pierde ámbito.
Una variable de nivel de procedimiento declarada con una instrucción conserva un valor hasta que el procedimiento termina de ejecutarse. Si el procedimiento llama a otros procedimientos, la variable conserva su valor mientras esos procedimientos se estén ejecutando.

Si se declara una variable de nivel de procedimiento con la palabra clave Static, la variable conserva su valor siempre que el código se esté ejecutando en cualquier módulo. Cuando todo el código ha terminado de ejecutarse, la variable pierde su ámbito y su valor. Su duración es la misma que la de la variable de nivel de módulo.

Las variables de nivel de módulo y las variables estáticas son diferentes. En un módulo estándar o en un módulo de clase, conserva su valor hasta que detenga la ejecución del código. En un módulo de clase, conserva su valor siempre que exista una instancia de la clase. Las variables de nivel de módulo consumen recursos de memoria hasta que restablezca los valores, así que úselas solo cuando sea necesario.

MEMORIA DINÁMICA

En muchas ocasiones no es posible conocer de antemano la cantidad de variables necesarias para un programa computacional, por ello existen aplicaciones que requieren de enormes cantidades de arreglos o datos por momentos breves en el funcionamiento del mismo, por lo que no es viable declarar de antemano a estas como variables, globales o locales de una función. Lo anterior implica emplear funciones de ANSI C que permiten reservar memoria de manera dinámica y ampliarla, reducirla o destruirla en tiempo de ejecución. El manejo de memoria dinámica es la base del poder del lenguaje C y le da la capacidad de crear programas complejos que emplean grandes cantidades de memoria y los maneja de manera eficiente.
Todos los programas definen variables que pueden ser definidas como globales y locales. Las variables globales y del programa principal (main) se almacenan en posiciones fijas de la memoria llamada memoria de datos. Las variables locales se almacenan en el segmento de memoria llamada pila y existen solo cuando se hace una invocación a la función que las declaro. También se pueden declarar variables estáticas locales que también se almacenan en segmentos fijos de memoria o en la memoria de datos, sin embargo, también están disponibles en la función que las declaro.
Todas estas variables comparten una característica en común, se definen cuando se compila el programa. Esto significa que el compilador reserva espacio en memoria para almacenar los valores para estas variables. Sin embargo, no todas las veces es posible conocer el número de variables con el que va a constar nuestro programa. C ofrece al desarrollador la opción de crear diferentes tipos de variables de forma dinámica, para crear tales variables se utilizan funciones como: malloc(), realloc(), calloc(), y free(). Las regiones de memoria que reservan/liberan estas funciones son almacenadas en el montículo o heap
Por lo regular cuando se diseña un algoritmo, se debe conocer que elementos de entrada tendrá y cuál será la salida, sin embargo, en algunas ocasiones no se sabe de forma exacta el número de variables que requerirá nuestro algoritmo.
El espacio de memoria asignado a una variable generada de manera dinámica se crea durante la ejecución del programa (tiempo de ejecución), al contrario de las variables declaradas en código, que el espacio de memoria se les asigna en tiempo de compilación. • Una variable que es generada dinámicamente, se construye (por ejemplo con malloc) y se puede destruir en tiempo de ejecución (uso de free).

Objeto: entidad existente en la memoria del ordenador que tiene unas propiedades (atributos o datos sobre sí mismo almacenados por el objeto) y unas operaciones disponibles específicas (métodos).
Clase: abstracción que define un tipo de objeto especificando qué propiedades (atributos) y operaciones disponibles va a tener.
Instanciación: e produce con la creación de un objeto perteneciente a una clase (se dice que se instancia la clase). El objeto que se crea tiene los atributos, propiedades y métodos de la clase a la que pertenece. Los objetos y sus características se usan en la construcción de programas, ya sea como contenedores de datos o como partes funcionales del programa
