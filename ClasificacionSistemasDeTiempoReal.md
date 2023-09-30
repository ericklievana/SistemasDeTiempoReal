---
title: Clasificacion de Sistemas de Tiempo Real
author: Erick Lievana Poy
---
# Clasificacion de Sistemas de Tiempo Real


Los sistemas de tiempo real, son procesos que dependen de ser finalizados en un intervalo de tiempo especifico, en base a esto podemos definir 3 tipos de sistemas de tiempo real en base a la consecuencia que se presenta cuando un proceso no termina en el plazo especificado:

* Sistema de tiempo real estricto
    * Todas las acciones deben terminar dentro del plazo especificado.
* Sistema de tiempo real firme
    * Se pueden perder plazos de manera ocasional
    * El valor de la respuesta disminuye con el tiempo
* Sistema de tiempo real flexible
    * Se pueden perder plazos de manera ocasional
    * Una respuesta tardia no tiene valor

## Clasificacion en base al comportamiento en caso de averia

En base a la reaccion del sistema cuando ocurre una falla

* Sistemas con parada segura
    * Detencion en estado seguro
    * Probabilidad de deteccion de fallos elevada

* Sistemas con degradacion aceptable
    * Funcionamiento con perdida parcial de funcionalidad o prestaciones
    * Tambien hay sistemas con tolerancia de fallos completa

## Clasificacion en base a su inicio

Los sistemas de tiempo real pueden clasificarse en base al detonante de su ejecucion

* Sistemas dirigidos por sucesos
    * Arranque cuando se produce un suceso de cambio de estado

* Sistemas dirigidos por tiempo
    * Arrangue en instantes de tiempos determinados

## Clasificacion en base a la arquitectura

Finalmente pueden clasificarse en base a su diseño y construcción:

* Centralizados: Los procesadores están localizados en un único nodo del sistema y la velocidad de comunicación entre procesadores es semejante a la velocidad del procesador.

* Distribuidos: Los procesadores están situados en distintos puntos del sistema y la velocidad de comunicación entre procesadores es muy baja respecto a su velocidad de proceso.

## Clasificacion de los ejemplos

### Monitor Cardiaco
Sistema de tiempo real estricto
Sistema de parada segura
Sistema dirigido por tiempo
Sistema centralizado

### Automoviles Autónomos
Sistema de tiempo real firme
Sistema de parada segura
Sistema dirigido por suceso
Sistema centralizado

### Habitat Automatizado
Sistema de tiempo real flexible
Sistemas con degradacion aceptable
Sistema dirigido por tiempo
Sistema distribuido

### Computadora de Vuelo
Sistema de tiempo real firme
Sistema de parada segura
Sistema dirigido por suceso
Sistema distribuido

### Sistema de Control de una Presa
Sistema de tiempo real estricto
Sistema de parada segura
Sistema dirigido por suceso
Sistema distribuido


# Referencias
1. De la Puente, J. A. (2000). Introducción a los Sistemas en Tiempo Real.
2. Mall, R. (2009). Real-time systems: theory and practice. Pearson Education India.
3. Ward, P. T. (1986). Structured development for real-time systems: Vol. I: Introduction and tools. Pearson Education.

