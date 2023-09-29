---
title: Clasificacion de Sistemas de Tiempo Real
author: Erick Lievana Poy
---
# Clasificacion de Sistemas de Tiempo Real

## Tipos de requisitos de temporales

* Tiempo real estricto
    * Todas las acciones deben terminar dentro del plazo especificado.
* Tiempo real flexible
    * Se pueden perder plazos de manera ocasional
    * El valor de la respuesta disminuye con el tiempo
* Tiempo real firme
    * Se pueden perder plazos de manera ocasional
    * Una respuesta tardia no tiene valor

Se distinguen por sus requisitos temporales y de fiabilidad

* Sistemas criticos (hard real-time systems)
    * Plazo de respuesta estricto
    * Comportamiento Temporal determinado por el entorno
    * Comportamiento en sobrecargas predecible
    * Requisitos de seguridad criticos
    * Redundancia activa
    * Volumen de datos reducidos

* Sistemas acriticos
    * Plazo de respuesta flexible
    * Comportamiento temporal determinado por el computador
    * Comportamiento en sobrecargas degradaddo
    * Requisitos de seguridad acriticos
    * Recuperacion de fallos
    * Gran volumen de datos

Se distinguen por su comportamiento en caso de averia

* Sistemas con parada segura
    * Detencion en estado seguro
    * Probabilidad de deteccion de fallos elevada

* Sistemas con degradacion aceptable
    * Funcionamiento con perdida parcial de funcionalidad o prestaciones
    * Tambien hay sistemas con tolerancia de fallos completa

Se distinguen por su grado de determinismo temporal

* Sistemas con respuesta garantizada
    * Comportamiento temporal garantizado analiticamente
    * Hace falta caracterizar con precision la carga maxima y posibles fallos

* Sistemas que hacen lo que pueden
    * Comportamiento temporal del tipo "lo mejor que se pueda"
    * No se hace una caracterizacion precisa de carga y fallos

Se distinguen por la cantidad de recursos disponibles

* Sistemas con recursos adecuados
    * Diseño con suficientes recursos para garantizar el comportamiento temporal con maxima carga y en caso de fallos

* Sistemas con recursos inadecuados
    * Diseño con recursos "razonables" desde un punto de vista económico

Se distinguen por la forma de arrancar la ejecución de sus actividades

* Sistemas dirigidos por sucesos
    * Arranque cuando se produce un suceso de cambio de estado

* Sistemas dirigidos por tiempo
    * Arrangue en instantes de tiempos determinados

Clasificación

Atendiendo al nivel de exigencia temporal, se pueden distinguir cuatro tipos de sistemas:

* Críticos: (hard real time systems) son aquellos en los que el tiempo de respuesta debe garantizarse a toda costa. Una respuesta tardía puede tener consecuencias fatales. Ej: Sistema de navegación de un avión.

* Esenciales: (soft real time systems) son aquellos sistemas con restricciones de tiempo en las que una respuesta tardía no produce graves daños pero si un deterioro del funcionamiento global. Ej: Sistema de comunicaciones (no se debe producir overflow en sistemas asíncronos, ni underflow en sistemas síncronos). Sistema de videoconferencia.

* Incrementales: la calidad de la respuesta obtenida depende del tiempo disponible para su cálculo. Si se les da más tiempo la respuesta mejora. Ej: Algoritmo de cálculo iterativo. Programa de ajedrez.

* No esenciales: corresponden con las tareas sin restricciones temporales.

Es posible que en un mismo sistema convivan procesos con distinto nivel de exigencia temporal. Un ejemplo claro es la labor de control de un proceso industrial y su monitorización. El control debe cumplir con exactitud las exigencias temporales (actual sobre válvulas, etc.), mientras que la presentación del estado del sistema para el operador puede sufrir un leve retraso.

Otros criterios de clasificación:

Atendiendo a la arquitectura hardware utilizada

* Propietarios: Desarrollados para un hardware específico y con un desarrollo particular para cada aplicación

* Abiertos: Basados en sistemas abiertos, incorporando estándares industriales: microprocesadores estándar, sistemas operativos estándar, protocolos de comuncaciones estándar y buses estándar. Atendiendo a la arquitectura del sistema

* Centralizados: Los procesadores están localizados en un único nodo del sistema y la velocidad de comunicación entre procesadores es semejante a la velocidad del procesador.

* Distribuidos: Los procesadores están situados en distintos puntos del sistema y la velocidad de comunicación entre procesadores es muy baja respecto a su velocidad de proceso.



# Referencias
1. De la Puente, J. A. (2000). Introducción a los Sistemas en Tiempo Real.

