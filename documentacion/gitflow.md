# Aplicación de Gitflow en el Sistema de Control de Rescate y Adopción Animal

## 1. Introducción

Gitflow es una forma de organizar el desarrollo de un proyecto de software mediante diferentes ramas de Git. Permite trabajar en nuevas funcionalidades sin modificar directamente la versión principal y mantener un historial de los cambios realizados.

En el Sistema de Control de Rescate y Adopción Animal se utilizó GitHub para organizar los archivos del proyecto, registrar los avances y aplicar un flujo de trabajo basado en Gitflow.

## 2. Organización de las ramas

Para desarrollar el proyecto se crearon las siguientes ramas:

**Rama master:** Representa la versión principal y estable del proyecto. Se mantiene separada de los cambios que todavía están en desarrollo.

**Rama develop:** Se utiliza para integrar los avances realizados antes de incorporarlos a la versión principal.

**Rama feature/diagramas-uml:** Se creó para trabajar con los diagramas UML de casos de uso, clases y secuencia, además de la arquitectura general del sistema.

**Rama feature/documentacion:** Se utiliza para elaborar la documentación de los patrones de diseño, los principios SOLID y el uso de Gitflow.

## 3. Desarrollo del proyecto mediante Gitflow

Primero se creó un repositorio público en GitHub con el nombre `Sistema-Rescate-Adopcion-Animal`.

Posteriormente, se configuró la rama principal `master` y se creó `develop` para integrar los avances del proyecto.

Desde `develop` se creó la rama `feature/diagramas-uml`, donde se subieron los cuatro diagramas realizados en Draw.io. Estos archivos se guardaron mediante un commit denominado "Agregar diagramas UML y arquitectura del sistema".

Después se creó el Pull Request #1 para integrar los cambios desde `feature/diagramas-uml` hacia `develop`. Una vez comprobado que no existían conflictos, se realizó el Merge correctamente.

Finalmente, se creó la rama `feature/documentacion`, donde se comenzaron a registrar las explicaciones de los patrones Singleton, Observer y Factory Method, los principios SOLID y la aplicación de Gitflow.

## 4. Uso de commits y Pull Requests

Los commits permiten guardar los avances y mantener un historial de los cambios realizados.

Por otra parte, los Pull Requests permiten revisar los archivos antes de integrarlos en otra rama.

En este proyecto se utilizó el Pull Request #1 para incorporar los diagramas UML a `develop`, demostrando cómo se pueden organizar e integrar los avances mediante Gitflow.

## 5. Justificación del uso de Gitflow

Gitflow se seleccionó porque permite organizar las diferentes actividades del proyecto y mantener separada la versión principal de los cambios en desarrollo.

Además, facilita identificar qué archivos se modificaron, cuándo se realizaron los cambios y cómo fueron integrados.

Esta forma de trabajo contribuye a mantener un mejor control de versiones, evitar modificaciones directas sobre la rama principal y facilitar el mantenimiento del proyecto.

## 6. Conclusión

La utilización de GitHub y Gitflow permitió organizar el desarrollo del Sistema de Control de Rescate y Adopción Animal. Mediante las ramas, los commits y los Pull Requests se pudo registrar el trabajo realizado y mantener un historial de los avances.

De esta manera, se comprendió la importancia del control de versiones y de utilizar un proceso ordenado para administrar los cambios de un proyecto de software.
