---
title: Sistemas de Tiempo Real
author: Erick Lievana Poy
---
# Sistemas de Tiempo Real

## Definición
En ingles Real Time Computing(RTC), se refiere a los sistemas de hardware y software los cuales deben de proporcionar una respuesta a un estímulo externo en un intervalo de tiempo finito y especificado. La garantía de un sistema de tiempo real depende tanto del resultado lógico de la operación y del tiempo transcurrido para la producción de resultados.

Los sistemas de tiempo real suelen estar integrados en sistemas de ingeniería mas complejos, en el que realizan funciones de control y/o monitorización, por ejemplo en sistemas empotrados(Embedded Systems).

## Características

Los sistemas de tiempo real, en general suelen compartir las siguientes características:

* Complejidad
> Debido a su necesidad de responder a estimulos externos, los sistemas de tiempo real son complejos para poder responder a diferentes estimulos de forma correcta.

* Concurrencia
> Son capaces de realizar multiples tareas al mismo tiempo, esto con el fin de cumplir el tiempo de respuesta.

* Dispositivos I/O
> De esta manera recibe los estimulos externos para iniciar sus procesos.

* Seguridad
> Deben ser sistemas seguros con multiples capas de contención para posibles fallas.

* Determinismo
> El sistema de tiempo real siempre proporcionara una respuesta dentro del tiempo asignado.

## Ejemplos

### Monitor Cardiaco
Es un sistema de tiempo real ya que recibe estimulos externos a traves de sensores, que son dispositivos I/O, tiene concurrencia ya que monitorea varios signos vitales, latidos por minuto, presion arterial, nivel de oxigenación, etc. Tiene varios sistemas de seguridad en caso de falla como la bateria en caso de falla electrica. Es complejo debido a que debe tener la lógica necesaria para poder interpretar las lecturas de los sensores y determinar si las lecturas son normales. Es determinista por que en cuanto realiza la lectura de los sensores, determina si estas son normales o no y en dado caso de que no lo sean emite una alarma de forma inmediata.

### Automoviles Autónomos
Recibe estimulos externos a traves de sensores, camaras, etc. Los estimulos externos son variados y de multiples direcciones y formas, peatones, otros automoviles, obstaculos en el camino, semaforos, etc. Es concurrente, puede recibir y reaccionar a multiples estimulos simultaneos, el propip control del vehiculo requiere de multiples acciones simultaneas. Es seguro ya que puede usar mas de un sensor para interpretar un mismo estimulo, tiene varios sistemas de redundancia para asegurar sus lecturas. Determinista ya que una vez recibido el estimulo cuenta con 1 segundo o menos para poder realizar una acción.

### Habitat Automatizado
Cuenta con diferentes sensores para detectar la temperatura, humedad, niveles de oxigeno, etc. Es complejo ya que hay factores relacionados y su acción para modificar 1 puede afectar a otros, por ejemplo modifica el nivel de humedad puede alterar la temperatura y son factores que se debe tener en cuenta. Es concurrente ya que puede realizar multiples tareas a la vez, como reducir la temperatura y reducir la humedad para evitar un congelemiento o matar a la especie que contiene. En cuanto a Seguridad, tiene varios sistemas de alarmas que al detectar algo fuera de lo comun dentro del habitar, se activan para indicarle a su cuidador, asi mismo si este puede resolver el problema con sus sistemas lo hara. Es determinista ya que reacciona a los cambios del habitat en intervalos de tiempo pequeños y siempre decide realizar una accion para mantener el habitat estable.

### Computadora de Vuelo
Recibe señales tanto de estimulos fuera y dentro del avion, temperatura, dirección y velocidad del viento, temperatura de los motores, nivel de combustible, localización, etc. Es concurrente ya que tiene que monitorear su estatus ademas de responder a los cambios externos, todo esto interpretando la señal de multiples sensores al mismo tiempo. Es complejo ya que cada uno de estos sistemas puede afectar al otro, por ejemplo al reducirse el nivel de combustible, tambien se reduce el peso del avion, por lo que la potencia requerida en los motores tambien es menor, la computadora de vuelo toma en cuenta todos estos factores para su funcionamiento. Es seguro ya que tiene varios sistemas de repuesto en caso de la falla de uno, por ejemplo hay aviones con sistemas de extintores en sus motores en caso dado de que estos fallen y empiecen a incendiarse y algunas computadoras de vvuelo tienen sensores para detectar la falla del motor y el incendio en este y activan los extintores automaticamente.

### Sistema de Control de una Presa
Tiene multiples sensores para detectar niveles de agua, nivel de producción de energia, nivel de flujo, estado de turbinas, etc. Es complejo por que una presa es una construcción compleja diseñada para controlar el nivel de agua de un caudal y generar energía por lo que el sistemas tiene multiples funciones. Es concurrente ya controla multiples caudales de entrada y de salida, controla el estado y la producción de energia de varias turbinas, controlar el estado de las turbinas por si mismo es un sistema de tiempo real, de igual forma el sistema controla la producción de energía y lo aumenta o disminuye segun sea el caso. Es seguro ya que cuenta con varias alarmas y mecanismos de control, bloqueo y seguridad para evitar accidentes o fallas, incluso cuenta con sistemas de respaldo en dado caso de que el principal falle, como por ejemplo desvia el caudal de agua a otra turbina en caso de que una falle. Es determinista ya que el monitoreo es constante y su reporte siempre tiene que ser en un intervalo de tiempo constante, asi mismo en casa de falla sus alarmas deben ser inmediatas.

## Referencias

* Alonso, A., & Crespo Lorente, A. (2010). Una panorámica de los Sistemas de Tiempo Real. Revista Iberoamericana de Automática e Informática Industrial, 3(2), 7-18.
* De la Puente, J. A. (2000). Introducción a los Sistemas en Tiempo Real.
* Castro Popoca, M., Águila Marín, F. M., Quevedo Nolasco, A., Kleisinger, S., Tijerina Chávez, L., & Mejía Sáenz, E. (2008). Sistema de riego automatizado en tiempo real con balance hídrico, medición de humedad del suelo y lisímetro. Agricultura técnica en México, 34(4), 459-470.Ben-Ari, Mordechai; "Principles of Concurrent and Distributed Programming", ch. 16, Prentice Hall, 1990, ISBN 0-13-711821-X, page 164
* Quiñonez, Y., Lizarraga, C., Peraza, J., & Zatarain, O. (2019). Sistema inteligente para el monitoreo automatizado del transporte público en tiempo real. Revista Ibérica de Sistemas e Tecnologias de Informacion, (31), 94-105.

