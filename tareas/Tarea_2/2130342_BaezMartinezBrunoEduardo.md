
## Software Development Life Cycle

El Ciclo de Vida del Desarrollo de Software (SDLC, por sus siglas en inglés) es un marco de trabajo conceptual utilizado en la ingeniería de software para gestionar proyectos de desarrollo. Describe un proceso estructurado que divide el desarrollo de software en una serie de etapas o fases distintas.

El propósito principal del SDLC es optimizar el proceso de desarrollo, asegurando que el producto final sea de alta calidad, cumpla con los requisitos del cliente y se entregue dentro del presupuesto y el cronograma establecidos. Proporciona un método para rastrear el progreso, asignar recursos de manera eficiente y gestionar la complejidad inherente a la creación de sistemas de software.

Este documento cubrirá las siete fases estándar del SDLC: Planificación, Análisis de Requisitos, Diseño, Implementación, Pruebas, Despliegue y Mantenimiento. Para cada fase, se detallará su objetivo principal, las actividades típicas, los entregables clave y los riesgos comunes asociados.

---

## Fases del SDLC

### 1. Planificación (Planning)

* **Objetivo:** Establecer las bases del proyecto. Define el alcance, los objetivos, los recursos necesarios (tiempo, personal, presupuesto) y la viabilidad técnica y económica del proyecto.
* **Actividades Típicas:**
    * Realizar estudios de viabilidad (técnica, económica, operativa).
    * Definir el alcance del proyecto (Project Scope).
    * Asignar recursos y estimar costos y plazos.
    * Crear un cronograma (ej. Diagrama de Gantt).
    * Identificar riesgos iniciales.
* **Entregables:**
    * Plan del Proyecto (Project Plan).
    * Estudio de Viabilidad.
    * Estimación de Costos y Cronograma.
* **Riesgos Comunes:**
    * **Scope Creep:** Expectativas poco claras que llevan a la expansión descontrolada del alcance.
    * Subestimación de recursos o tiempo.
    * Análisis de viabilidad deficiente que aprueba un proyecto inviable.

### 2. Análisis de Requisitos (Requirements/Analysis)

* **Objetivo:** Comprender y documentar detalladamente *qué* debe hacer el sistema. Es la fase crucial para capturar las necesidades de los stakeholders (clientes, usuarios finales).
* **Actividades Típicas:**
    * Realizar entrevistas, talleres y encuestas con los stakeholders.
    * Analizar los sistemas existentes.
    * Crear casos de uso e historias de usuario.
    * Documentar requisitos funcionales (lo que hace el sistema) y no funcionales (cómo funciona, ej. rendimiento, seguridad).
* **Entregables:**
    * Documento de Especificación de Requisitos de Software (SRS - Software Requirements Specification).
    * Casos de Uso o Historias de Usuario.
* **Riesgos Comunes:**
    * Requisitos ambiguos, contradictorios o incompletos.
    * Falta de participación del cliente o usuario final.
    * Falla en la gestión de cambios en los requisitos.

### 3. Diseño (Design)

* **Objetivo:** Definir *cómo* el sistema cumplirá con los requisitos. Se traduce el "qué" (requisitos) en un "cómo" (especificación técnica).
* **Actividades Típicas:**
    * **Diseño de Alto Nivel (Arquitectura):** Definir la arquitectura general, módulos principales, tecnologías (stacks) y plataformas.
    * **Diseño de Bajo Nivel (Detallado):** Diseñar componentes específicos, modelos de datos (esquemas de BBDD), algoritmos y diseño de la interfaz de usuario (UI/UX).
* **Entregables:**
    * Documento de Diseño de Software (SDD - Software Design Document).
    * Diagramas de arquitectura.
    * Diagramas Entidad-Relación (BBDD).
    * Wireframes, mockups y prototipos de UI/UX.
* **Riesgos Comunes:**
    * **Sobre-ingeniería:** Crear un diseño innecesariamente complejo.
    * Elegir una arquitectura que no es escalable o segura.
    * Ignorar los requisitos no funcionales (como el rendimiento) en el diseño.

### 4. Implementación (Implementation / Coding)

* **Objetivo:** Construir el software. Es la fase donde los desarrolladores escriben el código basándose en los documentos de diseño.
* **Actividades Típicas:**
    * Configurar los entornos de desarrollo (IDE, repositorios de código).
    * Programar (codificar) los módulos y componentes.
    * Realizar pruebas unitarias (Unit Testing) por parte de los desarrolladores.
    * Realizar revisiones de código (Code Reviews) entre pares.
* **Entregables:**
    * Código fuente (gestionado en un repositorio, ej. Git).
    * Binarios o ejecutables del software.
    * Resultados de las pruebas unitarias.
* **Riesgos Comunes:**
    * Mala calidad del código (difícil de mantener).
    * Incumplimiento de los estándares de codificación.
    * Problemas de integración entre diferentes módulos.

### 5. Pruebas (Testing)

* **Objetivo:** Verificar que el software funciona como se espera, cumple con los requisitos y está libre de defectos críticos antes de ser entregado al cliente.
* **Actividades Típicas:**
    * **Pruebas de Integración:** Asegurar que los módulos funcionan bien juntos.
    * **Pruebas del Sistema:** Probar el sistema completo contra los requisitos (SRS).
    * **Pruebas de Aceptación del Usuario (UAT):** El cliente/usuario valida el software.
    * Pruebas no funcionales (rendimiento, estrés, seguridad).
* **Entregables:**
    * Plan de Pruebas (Test Plan) y Casos de Prueba (Test Cases).
    * Reportes de bugs (Bug Reports).
    * Acta de aceptación (UAT Sign-off).
* **Riesgos Comunes:**
    * Cobertura de pruebas insuficiente (no se prueba todo).
    * Descubrimiento de defectos graves en etapas tardías.
    * Presión del cronograma que lleva a saltarse fases de prueba.

### 6. Despliegue (Deployment)

* **Objetivo:** Poner el software en producción para que los usuarios finales puedan utilizarlo.
* **Actividades Típicas:**
    * Preparar el entorno de producción (servidores, bases de datos).
    * Realizar la migración de datos (si es necesario).
    * Capacitar a los usuarios finales.
    * Ejecutar el plan de "Go-live" (lanzamiento).
* **Entregables:**
    * Sistema en producción (software funcional).
    * Documentación de usuario y manuales de capacitación.
    * Notas de la versión (Release Notes).
* **Riesgos Comunes:**
    * Fallos en el entorno de producción.
    * Corrupción de datos durante la migración.
    * Resistencia al cambio por parte de los usuarios.

### 7. Mantenimiento (Maintenance)

* **Objetivo:** Asegurar que el software siga funcionando correctamente y siga siendo relevante después de su lanzamiento.
* **Actividades Típicas:**
    * **Mantenimiento Correctivo:** Corregir bugs descubiertos en producción.
    * **Mantenimiento Adaptativo:** Actualizar el software para que funcione en nuevos entornos (ej. nuevos SO, navegadores).
    * **Mantenimiento Perfectivo:** Añadir nuevas características o mejorar el rendimiento según la retroalimentación del usuario.
* **Entregables:**
    * Parches (Patches) y actualizaciones (Updates).
    * Versiones nuevas del software.
    * Documentación actualizada.
* **Riesgos Comunes:**
    * **Deuda Técnica:** Modificaciones rápidas que degradan la calidad del código, haciendo el mantenimiento futuro más costoso.
    * Introducir nuevos errores (regresiones) al corregir otros.
    * Obsolescencia tecnológica del sistema.

---

## Conclusiones

La aplicación del SDLC, especialmente en sus formas más tradicionales como el modelo de Cascada (Waterfall), presenta tanto oportunidades como limitaciones significativas en contextos prácticos.

**Limitaciones:**
En un contexto académico, los proyectos suelen tener duraciones cortas y requisitos relativamente estables, lo que puede hacer que un SDLC completo parezca burocrático o excesivo. En el ámbito profesional moderno, especialmente en startups o desarrollo web, la rigidez del SDLC tradicional es su mayor limitación. Los mercados cambian rápidamente y los requisitos de los clientes evolucionan, lo que hace que un modelo secuencial estricto (donde el diseño debe estar 100% cerrado antes de codificar) sea poco práctico. Esto ha dado lugar a metodologías Ágiles (como Scrum o Kanban), que aplican ciclos de SDLC muy cortos (Sprints).

**Oportunidades:**
A pesar de sus limitaciones, la principal oportunidad del SDLC es la **estructura** y la **disciplina**. En mi contexto profesional, incluso al usar metodologías Ágiles, comprender las fases del SDLC es fundamental. Un "Sprint" no es más que un mini-SDLC (se planifica, se diseña, se implementa, se prueba). Para proyectos grandes, gubernamentales o de infraestructura crítica (ej. software bancario o médico), la estructura formal del SDLC es una oportunidad invaluable para gestionar el riesgo, asegurar la calidad y mantener una documentación exhaustiva, lo cual es vital para la regulación y el mantenimiento a largo plazo.

---

## Referencias

1.  Pressman, R. S., & Maxim, B. R. (2020). *Software Engineering: A Practitioner's Approach* (9th ed.). McGraw-Hill Education.
2.  Sommerville, I. (2016). *Software Engineering* (10th ed.). Pearson.
3.  Project Management Institute. (2021). *A Guide to the Project Management Body of Knowledge (PMBOK Guide)* (7th ed.).
4.  IEEE Computer Society. (2017). *ISO/IEC/IEEE 12207:2017 - Systems and software engineering -- Software life cycle processes*.
5.  Atlassian. (s.f.). *What is the Software Development Life Cycle (SDLC)?*. Recuperado de https://www.atlassian.com/continuous-delivery/principles/software-development-life-cycle

