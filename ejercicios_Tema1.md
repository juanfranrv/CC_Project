---
layout: ejercicios_Tema1
---

## Tema 1: Arquitecturas software en la nube ##

## Ejercicio 1 ##

**Buscar una aplicación de ejemplo, preferiblemente propia, y deducir qué patrón es el que usa. ¿Qué habría que hacer para evolucionar a un patrón tipo microservicios?**

La aplicación que he elegido ha sido [IDron Data Analyzer](https://github.com/juanfranrv/iDronDataAnalyzer) (mi TFG). 

El patrón que utiliza es MVC (Modelo-Vista-Controlador). 

Para evolucionar el patrón MVC a un patrón tipo microservicios, hay que modularizar el controlador en distintos microservicios de forma que estén conectados entre sí y con el cliente, gracias a una API REST. De esta forma, tenemos distintos microservicios separados entre sí y totalmente independientes que se encuentran comunicados con el sistema y el cliente a través de un sistema de API REST.

***

## Ejercicio 2 ##

**En la aplicación que se ha usado como ejemplo en el ejercicio anterior, ¿podría usar diferentes lenguajes? ¿Qué almacenes de datos serían los más convenientes?**

Para la parte BACK-END se ha utilizado Google App Engine junto con el lenguaje de programación Python. La base de datos es la DataStore de tipo NO-SQL proporcionada por Google.

Para la parte FRONT-END se han utilizado los lenguajes de programación HTML5 y CSS3, JAVASCRIPT (AJAX y JQUERY). 

Por lo tanto, se utilizan distintos lenguajes de programación para programar la aplicación web.

La base de datos que más se adapta al tipo de aplicación es NO-SQL, ya que hay una gran cantidad de datos que se reciben constantemente por lo que se requiere de la rapidez proporcionada por este tipo de bases de datos. Además, gracias a que funciona con JSON nos facilita el envío de datos por medio de API REST.

Concluyendo, la base de datos que más conviene es la DataStore debido que está perfectamente integrida con Google App Engine, simplificando el trabajo que tiene que realizar el usuario: despliegue de la base de datos, integración con el sistema, gestión de índices... Google nos simplifica considerablemente todas estas tareas.

***
