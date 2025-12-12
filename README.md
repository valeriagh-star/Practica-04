# Practica-04

## ✅ Objetivo

Esta práctica está diseñada como una extensión directa de la Práctica 02. Se busca implementar un sistema modular utilizando conceptos avanzados de la POO, como Clases Abstractas, Interfaces y Manejo de Excepciones, para gestionar diferentes tipos de usuarios (Administrador y Empleado) y manejar colecciones de datos de manera organizada. 

## ✍️ Descripción

En esta práctica se evaluó la correcta implementación de los conceptos mencionados en el objetivo. Se ha realizado una estructura de clases con la clase base Usuario (abstracta) y sus subclases Administrador y Empleado.

* **Puntos clave de la implementación:**
  
* **Clase Abstracta Usuario:** Define el comportamiento general, incluyendo atributos protegidos (Nombre, Correo, Rol) y un método abstracto para mostrar el menú (mostrarMenu()). Contiene constructores con y sin parámetros, aplicando validaciones estrictas en el constructor con parámetros. Esta clase no podrá ser instanciada directamente, sino que servirá como base para clases derivadas que implementen su comportamiento específico.

* **Subclases Administrador y Empleado:** Heredan de Usuario e implementan el método abstracto mostrarMenu(), cada uno mostrando un menú específico de acciones. Sus constructores invocan explícitamente al constructor de la clase padre (super(...)).

* **Validaciones:** Se implementan validaciones de entrada para Nombre de usuario (no vacío y ≥5 caracteres) y Correo electrónico (contiene @ y termina en .com), lanzando excepciones adecuadas (IllegalArgumentException) si no se cumplen las condiciones.

* **Interfaz ArregloInterface:** Define el conjunto de métodos que deben ser desarrollados en la clase para garantizar una estructura coherente y reutilizable en el manejo de listas.

* **Clase ManejadorLista:** Implementa la interfaz ArregloInterface para manejar operaciones sobre listas.

* **Estructura de Directorios y Paquetes:** Uso correcto de package e import, organizando las clases en directorios específicos (modulos/, Interfaces/).

