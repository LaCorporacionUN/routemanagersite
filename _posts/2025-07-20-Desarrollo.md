---
title: Desarrollo
date: 2025-07-20 20:00:00 -0500
categories: [proyecto, desarrollo]
tags: [desarrollo]     # TAG names should always be lowercase
description: Desarrollo del proyecto
media_subpath: /assets/desarrollo
mermaid: true
---

## Tecnologías

- Java para el desarrollo del backend utilizando el framework Spring Boot.
- PostgreSQL para la base de datos.
- JavaScript + CSS + React Framework para el desarrollo del front-end.
- Whatsapp para la comunicación del usuario con el sistema.

## Patrón de diseño

Se decidió que para el desarrollo del backend de la aplicación se iba a seguir el 	paradigma de
Modelo-Vista-Controlador, pues era el que más se ajustaba al caso de uso.

## Estructuras de datos

A continuación, se listan las estructuras de datos usadas para el desarrollo del proyecto

### Cola de Prioridad (Heap)
Se implementará una Cola de prioridad, parte de los requerimientos del programa es poder reportar incidentes
para saber si la ruta se retrasará, estos incidentes deben ser priorizados según una tabla para ser resueltos.

### Cola

Dado que no podemos enviar todas las peticiones a Whatsapp.js al mismo tiempo entonces implementaremos una
cola (FIFO) para que reciba las peticiones de Whatsapp y las encole para irlas enviando una a una

### Linked List

Haremos uso de una linked list para la creación de rutas con sus respectivos métodos de inserción y borrado
para el momento en que necesitemos crear una nueva ruta o editar la que ya tenemos.

## Esquema de funcionamiento del sistema

![Esquema de funcionamiento](funcionamiento.jpeg)
