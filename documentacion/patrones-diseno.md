# Patrones de diseño del Sistema de Control de Rescate y Adopción Animal

## 1. Introducción

En el diseño del Sistema de Control de Rescate y Adopción Animal se utilizaron tres patrones de diseño: Singleton, Observer y Factory Method. Estos patrones permiten organizar mejor las responsabilidades del sistema, facilitar la gestión de los rescates y mantener una estructura que pueda ampliarse en el futuro.

## 2. Patrón Singleton

**Propósito:** Garantizar que exista una única instancia de la clase encargada de gestionar los casos de rescate.

**Aplicación en el sistema:** Se utiliza en la clase `GestorCasosRescate`, que cuenta con el atributo `instancia` y el método `obtenerInstancia()`. De esta manera, los diferentes componentes pueden acceder al mismo gestor para administrar la información de los rescates.

**Justificación:** Este patrón se seleccionó para evitar la creación de varios gestores independientes y mantener un control centralizado de los casos registrados.

## 3. Patrón Observer

**Propósito:** Permitir que los responsables reciban notificaciones cuando se produzcan cambios importantes en los casos de rescate.

**Aplicación en el sistema:** La clase `GestorCasosRescate` mantiene una lista de observadores y utiliza el método `notificarObservadores()`. La clase `ResponsableAtencion` implementa la interfaz `ObservadorRescate` mediante el método `actualizar()`.

**Justificación:** Este patrón facilita la comunicación entre el gestor y los voluntarios o veterinarios, permitiendo informarles sobre nuevos rescates sin depender de una comunicación manual.

## 4. Patrón Factory Method

**Propósito:** Facilitar la creación de diferentes tipos de animales mediante una estructura común.

**Aplicación en el sistema:** Se utiliza la clase abstracta `CreadorAnimal`, que define el método `crearAnimal()`. Las clases `CreadorPerro`, `CreadorGato` y `CreadorFaunaSilvestre` permiten crear objetos correspondientes a cada tipo de animal.

**Justificación:** Este patrón se eligió porque el refugio registra diferentes especies. Su utilización permite organizar la creación de animales y facilita incorporar otros tipos en el futuro sin modificar toda la estructura del sistema.

## 5. Conclusión

La utilización de Singleton, Observer y Factory Method contribuye a organizar las responsabilidades del sistema. Singleton centraliza la gestión de los casos, Observer facilita las notificaciones a los responsables y Factory Method permite crear diferentes tipos de animales. En conjunto, estos patrones ayudan a plantear un diseño más organizado, reutilizable y fácil de mantener.
