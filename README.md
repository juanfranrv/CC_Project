## Máster profesional en Ingeniería Informática - Cloud Computing ##

## Información ##

Los drones están siendo noticia en todo el mundo, tanto por su uso bélico como también en el área de la ciencia y ayuda a la humanidad. Esta tecnología, sin tripulación, es cada vez más común. Se pronostica que se va a invertir en este área más de 100.000 millones de dólares en los próximos 5 años. 

El término correcto para referirse a ellos es UAV (Vehículo Aéreo no Tripulado) y mezclan lo más avanzado en el campo de la aeronáutica y la robótica, logrando acciones que ningún humano podría realizar. Son utilizados en tareas de diversa índole, es decir, desde tareas que pueden ser peligrosas para una persona hasta tareas que requieren un nivel de exactitud que solo logra la tecnología.

A pesar de las numerosas ventajas, existen problemas provocados por el uso de esta tecnología, como por ejemplo incidentes con aviones, inclusiones en aeropuertos o aeródromos... Cada país dispone de una legislación propia para drones que todos los usuarios deberían de conocer y cumplir. Sin embargo, los drones suelen volar donde no deben, pudiendo provocar conflictos y situaciones de riesgo. Los pilotos y operadores de drones no siguen la normativa, y los cuerpos de seguridad del Estado, muchas veces la desconocen y no saben cómo actuar.

En este proyecto se propone la solución de los problemas anteriores mediante la implementación de un sistema alojado en la nube cuyo objetivo consiste en informar al usuario sobre diversos aspectos relacionados con la seguridad de estos vehículos y en la captura de información meteorológica para poder volar de forma óptima. De esta forma, el usuario podrá volar su dron sin miedo a sanciones o poner en peligro a otras aeronaves o infraestructuras.

***

### Documentación técnica ###

A continuación se van a enumerar las tecnologías que se utilizarán para el desarrollo de la aplicación web y el despliegue:

**Aplicación web:**

Para la parte BACK-END se utilizará el framework Django junto con el lenguaje de programación Python. La base de datos será de tipo NO-SQL, MongoDB.

Para la parte FRONT-END se utilizará HTML5 y CSS3, JAVASCRIPT (AJAX y JQUERY). Puede que se utilice el framework ANGULARJS. Para los gráficos se utilizará la librería HIGHCHARTS y para los mapas la librería GOOGLE MAPS.

**Infraestructura virtual:**

Para la integración continua del proyecto se utilizará SHIPPABLE junto con SELENIUM para realizar los tests unitarios. 

Se utilizará DOCKER para crear un contenedor que nos permita instalar la aplicación junto con todas las dependencias en cualquier máquina.

Para el aprovisionamiento se utilizará ANSIBLE junto con VAGRANT para la creación de las máquinas virtuales necesarias para desplegar la aplicación web.

***

### Requisitos de la aplicación ###

La aplicación tendrá que cumplir los siguientes requisitos:

* [X] Monitorización y análisis de datos atmosféricos en tiempo real.  
* [X] Seguimiento del drone utilizando el GPS incorporado. Además, se mostrarán las zonas restringidas en el área por la que vaya circulando el dron: como aeropuertos o aeródromos más cercanos, núcleos urbanos o tráfico aéreo, alertando tanto por mensaje como por sonido si se invade alguna de ellas. Se podrá consultar la altura del terreno por el que va circulando el dron y la salida/puesta de sol (prohibición de circular por la noche).
* [X] Pronóstico de datos atmosféricos por horas o por días.
* [X] Almacenamiento de datos monitorizados para el posterior estudio de la misión. Estudio con gráficos.
* [X] Detección de los datos atmosféricos procedentes del METAR y TAFOR del aeropuerto más cercano por el que vaya circulando el drone en ese momento.
* [X] Datos como la altura, velocidad y coordenadas del dron estarán actualizados constantemente mientras el dron esté volando.
 
***
