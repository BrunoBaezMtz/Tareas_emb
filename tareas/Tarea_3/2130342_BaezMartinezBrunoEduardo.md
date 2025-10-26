
# Análisis de Metodologías Ágiles: Scrum, Kanban y Design Thinking


"Ágil" es un enfoque iterativo e incremental para la gestión de proyectos y el desarrollo de software. Se basa en la entrega de valor de forma temprana y continua, adaptándose a los cambios en lugar de seguir un plan rígido.

Surgió a principios de los 2000 (formalizado en el "Manifiesto Ágil" de 2001) como una respuesta directa a las fallas de los modelos tradicionales (como el modelo de Cascada o *Waterfall*). Estos modelos pesados eran lentos, burocráticos y fallaban en gestionar la incertidumbre y los requisitos cambiantes, resultando en software que, al ser entregado meses o años después, ya no satisfacía las necesidades del cliente.

Este documento explorará los principios fundamentales de la agilidad, profundizará en tres marcos de trabajo clave (Scrum, Kanban y Design Thinking), analizará sus ventajas y riesgos, y reflexionará sobre su aplicación práctica.

---

## Principios Ágiles: Valores y Fundamentos

La agilidad se sustenta en el **Manifiesto Ágil**, que prioriza cuatro valores clave:

1.  **Individuos e interacciones** sobre procesos y herramientas.
2.  **Software funcionando** sobre documentación exhaustiva.
3.  **Colaboración con el cliente** sobre negociación contractual.
4.  **Respuesta ante el cambio** sobre seguir un plan.

Estos valores se desglosan en 12 principios, cuyo impacto en la gestión del trabajo es profundo:

* **Impacto en la Gestión:** En lugar de una gestión jerárquica (Top-Down) donde se dictan tareas, la agilidad promueve **equipos auto-organizados y multifuncionales**.
* **Impacto en el Proceso:** Se reemplazan las fases largas y secuenciales por **ciclos cortos (iteraciones)** que producen incrementos de producto funcional.
* **Impacto en la Calidad:** La calidad se integra mediante la **retroalimentación constante** (del cliente y del equipo), en lugar de una única fase de "Pruebas" al final.
* **Impacto en el Valor:** El enfoque cambia de "completar el proyecto" a "maximizar el valor entregado" en el menor tiempo posible.

---

## Panorama de Marcos Ágiles

Aunque a menudo se usan indistintamente, "Ágil" es la mentalidad, mientras que Scrum, Kanban y DT son marcos (frameworks) que la implementan.

### Scrum
Es un marco prescriptivo (con roles, eventos y artefactos definidos) diseñado para gestionar el desarrollo de productos complejos en entornos con alta incertidumbre.
* **Cuándo elegirlo:** Ideal para el desarrollo de nuevos productos desde cero, proyectos de I+D, o cuando los requisitos son emergentes y es probable que cambien drásticamente.

### Kanban
Es un método visual para gestionar el flujo de trabajo. Se centra en la entrega continua, limitando el trabajo en progreso (WIP) para optimizar la eficiencia y reducir cuellos de botella.
* **Cuándo elegirlo:** Excelente para equipos de soporte, mantenimiento (Help Desk), operaciones (DevOps), o cualquier proceso donde el trabajo llega de forma continua y variable (tickets), y donde los "Sprints" de Scrum no tienen sentido.

### Design Thinking (DT)
No es un marco de desarrollo *per se*, sino un proceso centrado en el ser humano para la resolución creativa de problemas. Se enfoca en la empatía para entender al usuario y definir el problema *correcto* antes de construir la solución.
* **Cuándo elegirlo:** Usar *antes* de Scrum o Kanban (en la "Fase 0") para explorar un problema ambiguo, innovar, o asegurar que el producto que se va a construir realmente resuelve una necesidad del usuario.

---

## Ventajas y Riesgos del Enfoque Ágil

| Beneficios | Limitaciones y Riesgos | Trade-offs (El "Costo" de ser Ágil) |
| :--- | :--- | :--- |
| **Entrega temprana y continua de valor:** El cliente ve progreso funcional rápido. | **Requiere alta involucración del cliente:** Un cliente ausente o indeciso paraliza el proceso. | **Menor predictibilidad a largo plazo:** Es difícil dar una fecha y costo fijos al inicio (vs. Cascada). |
| **Alta adaptabilidad al cambio:** Los cambios de requisitos son bienvenidos, incluso tarde. | **Riesgo de "Scope Creep" (Corrupción del alcance):** Si no se gestiona bien, el proyecto nunca termina. | **La documentación "just-in-time"** puede ser insuficiente para industrias altamente reguladas (ej. farmacéutica). |
| **Visibilidad y transparencia:** Todos conocen el estado del trabajo y los impedimentos. | **Riesgo de "Agile de utilería" (*Cargo Cult*):** Adoptar las ceremonias (Dailys, Planning) sin la mentalidad (auto-organización, feedback). | **Requiere equipos maduros y multifuncionales:** La auto-organización es difícil y requiere confianza. |
| **Mejora de la calidad y moral del equipo:** El feedback constante y la retrospectiva mejoran el producto y el proceso. | **Difícil de escalar:** Aplicar agilidad a cientos de personas requiere marcos de escalado complejos (ej. SAFe, LeSS). | **La autonomía del equipo** puede chocar con las estructuras de gestión jerárquicas tradicionales. |

---

## Scrum

### Conceptos Base
* **Propósito:** Scrum es un marco de trabajo ligero que ayuda a personas, equipos y organizaciones a generar valor a través de soluciones adaptativas para problemas complejos.
* **Cuándo usarlo:** Cuando el "qué" se está descubriendo mientras se hace el "cómo". Es un proceso empírico basado en **Transparencia, Inspección y Adaptación**.

### Roles
* **Product Owner (PO):**
    * *Responsabilidad:* Maximizar el valor del producto resultante del trabajo del equipo. Es el único propietario y responsable de gestionar el **Product Backlog** (priorización, contenido, visibilidad).
    * *Error Frecuente:* El "PO ausente" (no disponible para el equipo) o el "PO por comité" (múltiples personas dando órdenes contradictorias).
* **Scrum Master (SM):**
    * *Responsabilidad:* Un líder servicial que ayuda al equipo y a la organización a entender y adoptar Scrum. Elimina impedimentos, facilita eventos y protege al equipo de interrupciones externas.
    * *Error Frecuente:* Actuar como "Jefe de Proyecto" (asignando tareas) o como "Secretario del equipo" (solo agendando reuniones).
* **Development Team (Equipo de Desarrollo):**
    * *Responsabilidad:* Un grupo auto-organizado y multifuncional de profesionales que tienen todas las habilidades necesarias para crear el Incremento del producto en cada Sprint.
    * *Error Frecuente:* "Mini-silos" dentro del equipo (ej. "yo solo hago backend", "ella solo hace pruebas") o dependencia de un "héroe" técnico.

### Artefactos (Los "Qués")
* **Product Backlog (PB):** La lista única, ordenada y emergente de *todo* lo que se conoce que es necesario en el producto. Es gestionada por el PO.
* **Sprint Backlog (SB):** El conjunto de ítems del PB seleccionados para el Sprint actual, más el plan del Equipo de Desarrollo para entregar el Incremento.
* **Incremento (Increment):** La suma de todos los ítems del Product Backlog completados durante un Sprint (y Sprints anteriores). Debe ser *usable* y cumplir con la **Definition of Done**.

#### Criterios de Calidad: DoD vs. Criterios de Aceptación

* **Definition of Done (DoD):** Es un *checklist global de calidad* que aplica a *todos* los ítems del backlog. Es la definición compartida de "terminado".
    * *Ejemplo de DoD:* "Pasa todas las pruebas unitarias", "Código revisado por pares (Peer Review)", "Documentación de la API actualizada", "Probado en entorno de Staging".
* **Criterios de Aceptación (AC):** Son *específicos de un ítem* (Historia de Usuario). Definen el comportamiento funcional esperado desde la perspectiva del usuario.
    * *Ejemplo de AC (para un login):* "Usuario puede iniciar sesión con email y contraseña correctos", "Usuario ve mensaje 'Email o contraseña inválidos' si falla", "Usuario no puede hacer clic en 'Login' si los campos están vacíos".

### Eventos (Los "Cuándos")
* **El Sprint:**
    * *Objetivo:* El corazón de Scrum. Un *time-box* (caja de tiempo) de un mes o menos (comúnmente 2 semanas) durante el cual se crea un Incremento de producto "Terminado", usable y potencialmente desplegable.
* **Sprint Planning (Planificación):**
    * *Objetivo:* Definir el trabajo a realizar en el Sprint. Responde: 1. ¿*Qué* valor se entregará (Sprint Goal)? 2. ¿*Qué* ítems del PB se seleccionan? 3. ¿*Cómo* se realizará el trabajo?
    * *Duración:* Máx. 8 horas para un Sprint de 1 mes.
    * *Antipatrón:* El PO o un gerente *impone* el Sprint Backlog al equipo sin que este negocie o estime el esfuerzo.
* **Daily Scrum (Scrum Diario):**
    * *Objetivo:* Una reunión de 15 minutos para el Equipo de Desarrollo para inspeccionar el progreso hacia el Sprint Goal y adaptar el plan del día. (No es para el PO o el SM).
    * *Duración:* 15 minutos (fijos).
    * *Antipatrón:* Convertirlo en un "reporte de estatus" para el Scrum Master o el PO, en lugar de una sincronización del equipo.
* **Sprint Review (Revisión):**
    * *Objetivo:* Inspeccionar el Incremento (el "qué" se construyó) y adaptar el Product Backlog. Se presenta el trabajo "Terminado" (la "demo") a los stakeholders para obtener feedback.
    * *Duración:* Máx. 4 horas para un Sprint de 1 mes.
    * *Antipatrón:* Una "demo" pasiva donde el equipo solo muestra y los stakeholders no interactúan. O peor, mostrar trabajo "casi terminado".
* **Sprint Retrospective (Retrospectiva):**
    * *Objetivo:* Inspeccionar al equipo, sus interacciones y el proceso (el "cómo" trabajaron). El objetivo es generar un plan de mejora (ej. "Qué empezar a hacer", "Qué dejar de hacer", "Qué seguir haciendo").
    * *Duración:* Máx. 3 horas para un Sprint de 1 mes.
    * *Antipatrón:* Una sesión de quejas sin generar acciones concretas y asignables, o culpar a personas fuera del equipo.

### Métricas
* **Velocity (Velocidad):**
    * *Qué es:* La cantidad de trabajo (medido en Puntos de Historia) que un equipo completa (según su DoD) en un Sprint.
    * *Interpretación:* Es un indicador *histórico* que ayuda al equipo a *pronosticar* cuánto trabajo puede asumir en futuros Sprints.
    * *Cómo NO usarla:* Como medida de productividad, para comparar equipos, o para establecer objetivos ("este Sprint deben hacer 30 puntos").
* **Burndown Chart (Gráfico de Avance):**
    * *Qué es:* Un gráfico que muestra el trabajo restante (eje Y) contra el tiempo (eje X) del Sprint.
    * *Interpretación:* Ayuda al equipo a visualizar su progreso hacia el Sprint Goal. Si la línea real está muy por encima de la ideal, el equipo está en riesgo de no terminar.
* **Work In Progress (WIP):**
    * *Qué es:* (Más común en Kanban, pero aplicable a Scrum). La cantidad de tareas que están "En Progreso" simultáneamente.
    * *Interpretación:* Un WIP alto es señal de multitarea y cuellos de botella. Limitar el WIP (ej. "cada desarrollador solo puede tener una tarea activa") mejora el foco y la velocidad de entrega.

---

## Kanban

### Fundamentos: Principios y Prácticas

Kanban es un método de gestión de flujo evolutivo.

* **Principios Fundacionales (Cambio):**
    1.  **Empezar con lo que se hace ahora:** No hay cambios drásticos. Se visualiza el proceso actual.
    2.  **Acordar buscar la mejora evolutiva:** Pequeños cambios incrementales.
    3.  **Respetar los procesos, roles y responsabilidades actuales:** Kanban no impone roles (como SM o PO).
* **Prácticas Clave (Operación):**
    1.  **Visualizar el trabajo:** Usar un tablero (Tablero Kanban).
    2.  **Limitar el Trabajo en Progreso (WIP):** ¡La práctica más importante!
    3.  **Gestionar el Flujo:** Medir y optimizar cómo el trabajo fluye por el sistema.
    4.  **Hacer las Políticas Explícitas:** (Ej. ¿Qué significa "Listo"? ¿Cómo se prioriza?).
    5.  **Establecer Bucles de Retroalimentación:** (Ej. Reuniones de revisión de flujo, Dailys).
    6.  **Mejorar Colaborativamente (usando modelos):** Evolucionar el proceso.

### Tablero Kanban y Límites WIP

Un tablero Kanban visualiza las etapas del flujo de trabajo.

**Propuesta de Columnas (Equipo de Desarrollo):**

| `Backlog` | `Listo para Analizar` | `Análisis` (WIP: 2) | `Listo para Desarrollo` | `Desarrollo` (WIP: 4) | `Revisión/Pruebas` (WIP: 2) | `Listo para Desplegar` | `Desplegado` |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |

**Límites WIP Razonados:**

* **`Análisis` (WIP: 2):** Limita a que el equipo no analice más de 2 ítems a la vez. Evita crear un gran backlog de trabajo "listo para desarrollar" que se vuelve obsoleto.
* **`Desarrollo` (WIP: 4):** Si el equipo tiene 4 desarrolladores, un límite de 4 (o 3) fomenta el *single-tasking*. Si se alcanza el límite, un desarrollador libre debe ayudar a *desbloquear* ítems en `Revisión/Pruebas` en lugar de tomar trabajo nuevo.
* **`Revisión/Pruebas` (WIP: 2):** Evita que el equipo de QA (Calidad) se sature. Si el WIP está lleno, los desarrolladores deben parar y ayudar a probar.

El objetivo del WIP es **dejar de empezar y empezar a terminar**.

### Métricas de Flujo
Kanban se obsesiona con la eficiencia del flujo.

* **Lead Time (Tiempo de Entrega):** Tiempo total desde que un cliente *pide* algo hasta que lo *recibe*. (Perspectiva del cliente).
* **Cycle Time (Tiempo de Ciclo):** Tiempo total desde que el equipo *empieza a trabajar* en algo hasta que lo *termina*. (Perspectiva del equipo).
* **Throughput (Rendimiento):** El número de ítems de trabajo completados por unidad de tiempo (ej. "Entregamos 8 tickets por semana").
* **Diagrama de Flujo Acumulado (CFD - Cumulative Flow Diagram):**
    * *Qué es:* Un gráfico de áreas apiladas que muestra cuántos ítems hay en cada columna del tablero a lo largo del tiempo.
    * *Lectura:*
        * La banda superior (ej. `Desplegado`) muestra el Throughput.
        * Una banda que se *ensancha* (ej. la banda de `Pruebas` crece) indica un **cuello de botella**: el trabajo entra más rápido de lo que sale de esa fase.
        * Una banda que se *aplana* indica trabajo bloqueado o falta de actividad.

### Políticas y Clases de Servicio
* **Políticas Explícitas:** Son las "reglas del juego" visibles para todos.
    * *Ejemplo:* "Definición de 'Listo para Analizar': El PO ha validado el requerimiento", "Política de bloqueo: Mover la tarjeta a 'Bloqueado' y añadir etiqueta roja", "Prioridad: Las tarjetas en `Revisión` siempre se atienden antes que las de `Desarrollo`".
* **Clases de Servicio (CoS):** Definen cómo se prioriza el trabajo entrante.
    * *Ejemplo de CoS:*
        * **Expedite / Urgente (ej. Bug en producción):** (WIP: 1). Pasa por delante de todo lo demás.
        * **Fecha Fija (Fixed Date):** (ej. Requerimiento legal para fin de mes). Debe terminarse en una fecha específica.
        * **Estándar (Standard):** Trabajo normal, se atiende por orden (FIFO - First In, First Out).
        * **Intangible (ej. Deuda técnica):** Importante pero no urgente. Se hace cuando hay capacidad.

### Cuándo usar Kanban
* Cuando el trabajo es impredecible o altamente variable (tickets de soporte, mantenimiento).
* Cuando el equipo necesita entregar valor de forma continua, no en lotes (Sprints).
* Cuando se quiere mejorar un proceso existente sin la disrupción de adoptar Scrum (roles, eventos).
* Para equipos de operaciones (DevOps) que gestionan infraestructura y despliegues.

---

## Design Thinking (DT)

### Visión General y Principios
Design Thinking (DT) es un proceso iterativo de resolución de problemas centrado en el ser humano.

* **Principios:** 1. **Centrado en el Humano** (Empatía), 2. **Colaborativo** (Multidisciplinario), 3. **Iterativo** (Prototipar y probar), 4. **Acción/Prototipado** ("Construir para pensar").
* **Encaje con Software:** DT es la herramienta perfecta para la fase de **Descubrimiento de Producto (Product Discovery)**. Mientras Ágil (Scrum/Kanban) se enfoca en *construir la cosa correctamente*, Design Thinking se enfoca en *construir la cosa correcta*.

### Fases del Proceso
(Modelo de 5 fases de la d.school de Stanford)

**1. Empatizar (Empathize):**
* *Objetivo:* Entender profundamente al usuario, sus necesidades, motivaciones y contexto.
* *Técnicas:* Entrevistas (no encuestas), observación (shadowing), Mapa de Empatía.
* *Entregables:* *Insights* (descubrimientos), *Personas* (arquetipos de usuario).

**2. Definir (Define):**
* *Objetivo:* Sintetizar los hallazgos de la empatía para articular un problema claro y accionable.
* *Técnicas:* Declaración de Punto de Vista (POV: "Usuario... necesita... porque..."), Preguntas "How Might We...?" (HMW - ¿Cómo podríamos...?).
* *Entregables:* Un POV claro, set de preguntas HMW priorizadas.

**3. Idear (Ideate):**
* *Objetivo:* Generar un gran volumen y variedad de soluciones potenciales al problema definido. (Cantidad > Calidad en esta fase).
* *Técnicas:* Brainstorming (Lluvia de ideas), Crazy 8s (8 ideas en 8 minutos), SCAMPER.
* *Entregables:* Conjunto amplio de ideas, filtradas y priorizadas (ej. por matriz de Impacto vs. Viabilidad).

**4. Prototipar (Prototype):**
* *Objetivo:* Crear representaciones de baja fidelidad de las soluciones para obtener feedback. Es "construir para pensar", no "construir para lanzar".
* *Técnicas:* Bocetos en papel (Paper prototypes), Wireframes (Balsamiq, Figma), Storyboards, maquetas físicas (con cartón, Lego).
* *Entregables:* Un prototipo de baja o media fidelidad.

**5. Probar (Test):**
* *Objetivo:* Poner el prototipo en manos de usuarios reales para obtener feedback. El objetivo es refinar el prototipo y, a veces, redefinir el problema.
* *Técnicas:* Pruebas de usabilidad ("Piensa en voz alta"), Entrevistas de feedback.
* *Entregables:* Feedback validado, insights sobre qué iterar.



---

## Conclusiones

La agilidad no es una "bala de plata", sino un cambio de mentalidad fundamental que prioriza la adaptación y la entrega de valor.

En mi contexto académico, la aplicación de estos marcos ofrece oportunidades claras. Los proyectos semestrales se beneficiarían enormemente de **Scrum**, utilizando Sprints de 2 semanas para evitar la procrastinación y asegurar una entrega funcional (un Incremento) para mitad de semestre, en lugar de un esfuerzo masivo la última semana.

**Design Thinking** es crucial en la etapa de definición de proyectos de tesis o investigación. Aplicar Empatía y Definición aseguraría que la pregunta de investigación sea relevante y esté bien enmarcada antes de dedicar meses al desarrollo.

En un contexto profesional, **Kanban** parece ser la herramienta más versátil para el trabajo diario, gestionando el flujo constante de tareas (correos, reportes, mantenimiento de código), mientras que **Scrum** es el motor para la creación de nuevos productos. La verdadera madurez ágil radica en saber qué marco aplicar (o combinar) según el contexto del problema.

---

## Referencias

1.  Beck, K., et al. (2001). *Manifesto for Agile Software Development*. Agile Manifesto. Recuperado de https://agilemanifesto.org/
2.  Schwaber, K., & Sutherland, J. (2020). *La Guía de Scrum*. Recuperado de https://scrumguides.org/
3.  Anderson, D. J. (2010). *Kanban: Successful Evolutionary Change for Your Technology Business*. Blue Hole Press.
4.  IDEO. (s.f.). *Design Thinking*. Recuperado de https://designthinking.ideo.com/
5.  Atlassian. (s.f.). *Agile Coach: What is Agile?*. Recuperado de https://www.atlassian.com/agile

