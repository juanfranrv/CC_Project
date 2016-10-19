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

