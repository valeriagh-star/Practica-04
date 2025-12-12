# Practica-04 

## ✅ Objetivo
<div align="justify">
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

## ⚙️ Tecnologías utilizadas

* **Lenguaje:** JavaSE-24.
* **IDE:** Eclipse IDE.

## 📁 Estructura del Proyecto

El proyecto está organizado en la siguiente estructura de directorios:

**Proyecto/**
  
  **├── src/**

  **│   ├── modulos/**
  
  **│   │      ├── Administrador.java**
 
  **│   │      ├── Empleado.java**
  
  **│   │      └── Usuario.java**

  **│   ├── Interfaces/**
  
  **│   │      └── ArregloInterface.java**
 
  **│   ├── Main.java**

  **│   └── ManejadorLista.java**
  
  **└── README.txt**

## 📸 Evidencias (Capturas de pantalla)

A continuación se muestran capturas de pantalla sobre la ejecución en consola, donde se verifica el funcionamiento de las validaciones en los menús de Administrador y Empleado, el manejo de excepciones al intentar crear un usuario con datos inválidos, y el uso de las funcionalidades de ManejadorLista.

![Captura 1 de la Ejecución de Main](practica04(1).png)
![Captura 2 de la Ejecución de Main](practica04(2).png)

El código fuente de los directorios está organizado por paquetes y se puede revisar directamente en la carpeta [src/](https://github.com/valeriagh-star/Practica-04/tree/main/src).

| Carpetas | Ruta del Archivo .java |
| :--- | :--- |
| **Clase Usuario** | [src/modulos/Usuario.java](https://github.com/valeriagh-star/Practica-04/blob/main/src/modulos/Usuario.java) | 
| **Clase Administrador** | [src/modulos/Administrador.java](https://github.com/valeriagh-star/Practica-04/blob/main/src/modulos/Administrador.java) |
| **Clase Empleado** | [src/modulos/Empleado.java](https://github.com/valeriagh-star/Practica-04/blob/main/src/modulos/Empleado.java) |
| **Interfaz ArregloInterface** | [src/Interfaces/ArregloInterface.java](https://github.com/valeriagh-star/Practica-04/blob/main/src/Interfaces/arregloInterface.java) | 
| **Clase Main** | [src/Main/Main.java](https://github.com/valeriagh-star/Practica-04/blob/main/src/Main.java) |
| **Clase ManejadorLista** | [src/ManejadorLista/ManejadorLista.java](https://github.com/valeriagh-star/Practica-04/blob/main/src/ManejadorLista.java) |
| **README** | [Practica04/main/README.txt](https://github.com/valeriagh-star/Practica-04/blob/main/README.txt) | 

## ▶️ Instrucciones de ejecución

1.  **Clonar/Importar el repositorio el Repositorio:** Importa la carpeta Proyecto como un proyecto Java existente en Eclipse o IntelliJ.
2.  **Abrir Main:** Localiza el archivo src/Main.java.
3.  **Ejecutar:** Haz clic derecho sobre src/Main.java y selecciona "Run As" -> "Java Application".
4.  **Interacción:** El programa solicitará el Nombre, Correo y Rol (Empleado o Administrador) para crear un nuevo usuario. El programa manejará las validaciones automáticamente (Manejo de Excepciones) para el nombre de usuario (mínimo 5 caracteres) y el formato del correo electrónico (@ y .com). Se mostrará el menú correspondiente al Rol ingresado (Administrador o Empleado).
</div>
