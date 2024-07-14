Variables:
En Kotlin, las variables se definen usando la palabra clave var. Estas variables pueden cambiar su valor después de haber sido inicializadas. Por ejemplo:

kotlin
Copiar código
var nombre = "Juan"
nombre = "Pedro"  // Cambiando el valor de la variable 'nombre'
Constantes:
Las constantes en Kotlin se definen usando la palabra clave val. Estas son variables inmutables cuyo valor no puede cambiar después de la inicialización. Por ejemplo:

kotlin
Copiar código
val pi = 3.14159
// pi = 3.14 // Esto dará un error, ya que 'pi' es una constante
Opcionales (Variables nulas):
En Kotlin, todas las variables por defecto son no nulas, lo que significa que no pueden contener un valor nulo a menos que se especifique explícitamente. Para definir una variable que pueda contener un valor nulo, se usa el operador ? al final del tipo de datos. Por ejemplo:

kotlin
Copiar código
var edad: Int? = null // Variable que puede ser nula
Nulos:
Kotlin tiene un sistema de tipos que ayuda a prevenir los errores de referencia nula (NullPointerException) que son comunes en otros lenguajes de programación. Esto se logra definiendo tipos que pueden o no contener valores nulos.

Tipos no nulos: Como se mencionó, las variables normales en Kotlin no pueden contener valores nulos a menos que se especifique explícitamente con el tipo seguido de ?.

Operaciones seguras con nulos: Kotlin proporciona operaciones seguras para trabajar con variables que pueden ser nulas, utilizando el operador ?. para llamar métodos o acceder a propiedades en una variable que puede ser nula sin causar una excepción.

Elvis operator (?:): Se utiliza para proporcionar un valor predeterminado en caso de que la expresión a la izquierda sea nula. Por ejemplo:

kotlin
Copiar código
val longitud: Int = nombre?.length ?: 0
Aquí, nombre?.length devuelve la longitud de nombre si no es nulo, y 0 si nombre es nulo.
