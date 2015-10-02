# ReporteID150154

Reporte: Lenguajes y paradigmas de la programación

Itzel Tlelo Coyotecatl

ID 150154
 
Variables estáticas

Son propias únicamente de la clase y no de los objetos que pueden llegar a crearse de la misma, por lo tanto, sus valores son compartidos por todos los objetos de la clase. Para invocarla no se necesita crear un objeto de la clase en la que se define, basta con escribir su nombre si es invocada desde la misma clase. Si es invocada desde una clase distinta, debe anteponerse a su nombre, el de la clase en la que se encuentra seguido del operador punto
<NombreClase>.variableEstatica
Generalmente suelen emplearse para definir constantes comunes a todos los objetos de la clase.

Ciclo de vida de las variables

Variables de instancia (u objeto): Se crean cuando se crea el objeto que las contiene. Se inicializan por defecto si no se hace de modo explícito (ej. 0 para números, “false” para booleano, “null” para objetos). Se destruyen cuando el recolector de basura de Java no encuentra referencias activas para el objeto.
Variables estáticas (o de clase): Se crean cuando la clase se usa por primera vez. Se inicializan por defecto. Suelen existir para el resto del programa (salvo que no esté cargado).
Variables locales (o de bloque): Creadas en la sentencia en la que están definidas. No se inicializan por defecto. Contienen datos imprevisibles. Se destruyen al salir del bloque (en la llave final)

Memoria dinámica

Es un espacio de almacenamiento que solicita en tiempo de ejecución. A medida que el proceso va necesitando espacio va solicitando más memoria al sistema. El medio para manejar la memoria que otorga el sistema operativo, es el puntero, puesto que no se sabe el tiempo de compilación.

Los datos se crean y destruyen mientras se ejecuta el programa y por lo tanto la estructura se va dimensionando conforme lo requiera el programa. Generalmente la memoria dinámica trabaja dividiendo el programa en texto, datos (estáticos), pila y una zona libre o heap. 

Las ventajas de su uso son: disposición de sistema que dependa de información dinámica, la memoria puede incrementarse según se requiera, es memoria reservada en tiempo de ejecución por lo tanto su tamaño puede variar durante la ejecución del programa. Las desventajas son: es difícil de implementar en estructuras complejas como la recursividad, es difícil de manejar, la memoria dinámica puede afectar el rendimiento de la ejecución del programa, se deben llevar a cabo distintas tareas por lo que representa una carga adicional que dependerá de la implementación.

Clase

Abstracción que define un tipo de objeto especificado qué propiedades (atributos) y operaciones disponibles va a tener.

Objeto

Entidad existente en la memoria del ordenador que tiene unas propiedades (atributos o datos sobre sí mismo almacenados por el objeto) y unas operaciones disponibles específicas (métodos).

Instanciación

Puede decirse que un objeto es una instancia de una clase. En general varios objetos de una misma clase constituyen instancias múltiples de la clase. 

Herencia

Permite compartir automáticamente métodos y datos entre clases, subclases y objetos. La herencia contiene Clase padre o “Superclase” y Clase(s) hija(s) o “Sub Clase(s)”

Sobrecarga

Es la creación de varios métodos con el mismo nombre pero con diferentes firmas y definiciones. Por ejemplo, en Java los métodos se diferencian de acuerdo a sus parámetros.

Ensombrecimiento (shadowing)

Se le llama así al hecho de que en una clase una variable miembro y una local definida en un método miembro, se llamen igual.

Ciclo de vida de variables de clase

Clase: Una clase también es un objeto dentro de la máquina virtual, se caracteriza por contener los bytecodes con el código ejecutable resultante de su compilación. Además contiene las variables estáticas definidas en la clase. La clase es cargada por la máquina virtual cuando se detecta alguna dependencia con otra clase que la utiliza. Una vez cargada se inicializan sus atributos estáticos y se ejecuta el código que contenga. Una clase existirá mientras ésta sea referenciada por un cargador de clases. Por lo tanto la clase y sus atributos permanecerán en memoria hasta la destrucción de la máquina virtual.
 
Referencia

aine31. (2013). ¿Qué es shadowing?. Sitio web disponible en https://misapuntesdeprogramacion.wordpress.com/2013/01/17/que-es-shadowing/

Adrian. (2011). ESTRUCTURA DE DATOS. MEMORIA ESTATICA Y DINAMICA. Sitio web disponible en http://adrian-estructuradedatos.blogspot.mx/2011/04/memoria-estatica-y-dinamica.html

adrformacion. (2015). Curso de Java. Variables estáticas o de clase. Página web disponible en http://www.adrformacion.com/cursos/java/leccion2/tutorial8.html

Aprenderaprogramar. (2015). Conceptos de objetos y clases en Java. Definición de instancia. Ejemplos básicos y prácticos. (CU00619B). Sitio web disponible en http://www.aprenderaprogramar.com/index.php?option=com_content&view=article&id=411:conceptos-de-objetos-y-clases-en-java-definicion-de-instancia-ejemplos-basicos-y-practicos-cu00619b&catid=68:curso-aprender-programacion-java-desde-cero&Itemid=188

Diego Franco. (2014). HERENCIA Y SOBRECARGA EN JAVA. Prezi. Sitio web disponible en https://prezi.com/mfmez0jij89m/herencia-y-sobrecarga-en-java/

Sin autor. (s.f). 1.00 Clase 11 Ámbito y acceso. Documento PDF disponible en http://mit.ocw.universia.net/1.00/s02/class-sessions/lecture-11/lecture-11.pdf
