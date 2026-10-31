Análisis Técnico, de Mercado y de Viabilidad

1. Análisis de Mercado (¿Qué hay ahí fuera?)
Para justificar la viabilidad de CÓRTEX, se ha realizado un estudio de las soluciones existentes, concluyendo que **ninguna une los tres componentes necesarios** (detección, entrenamiento y certificación de autonomía):

*   **Plataformas de Retos (HackerRank, CodeChef):** Se centran en evaluar el resultado final (el código funciona), pero no detectan si el usuario ha usado IA ni entrenan el pensamiento a largo plazo. Su modelo es B2B (vender exámenes a empresas).
*   **Apps de Bienestar Digital (Opal, Forest, Screen Time):** Se basan en el bloqueo paternalista. No resuelven el problema del pensamiento crítico, solo limitan el tiempo de pantalla. Tienen un modelo de negocio de suscripción que depende de que el usuario siga enganchado a la app.
*   **Herramientas de Detección de IA:** Existen detectores de texto generado por IA, pero son pasivos. No ofrecen un plan de entrenamiento ni una mejora medible.

**El hueco del mercado:** Nadie ha construido un "gimnasio cognitivo" unificado. Cada actor del mercado está optimizado para un solo componente (detección, bloqueo o evaluación). La unificación requiere un modelo de negocio disruptivo: **que el éxito de la app sea hacer que el usuario la abandone.**

2. Análisis Técnico (¿Cómo se va a construir?)
El proyecto se desarrollará como una aplicación nativa para Android para aprovechar el conocimiento previo en el ecosistema y el máximo control sobre las APIs del sistema.

*   **Lenguaje de programación:** Kotlin (aprovechando la familiaridad con Java/C++) y diseño de interfaces con XML (Android clásico).
*   **Backend y Base de Datos:** Firebase (Authentication para el login y Firestore para guardar los informes de autonomía y los datos del usuario).
*   **Motor de Ejecución de Código:** API de Judge0. Esta API permitirá compilar y ejecutar el código que el usuario escriba en la "Sala de Apagón" (Java, C++, etc.) en un entorno seguro (sandbox), evitando cualquier riesgo de malware para la app o el dispositivo.
*   **Lógica de Detección (MVP):** Para la primera versión, el bloqueo del copiar/pegar se implementará mediante la configuración del `EditText` en Android. La detección de patrones de tecleo se simulará midiendo el tiempo de escritura y los intentos de pegado, generando un informe básico de autonomía.

3. Análisis de Viabilidad y Modelo de Negocio
*   **Viabilidad Técnica:** Alta. Las tecnologías elegidas (Kotlin, Firebase, Judge0) son estándar en la industria y cuentan con documentación abundante.
*   **Modelo de Negocio (Futuro):** Al ser una app diseñada para volverse innecesaria, el modelo de suscripción tradicional (SaaS) no encaja. La monetización podría venir por:
    *   **Informes de Autonomía (B2C):** Pago único por la generación de un informe técnico detallado que el usuario pueda adjuntar a su CV o LinkedIn como prueba de sus habilidades reales sin IA.
    *   **Licencias B2B (Universidades y Empresas):** Venta de la plataforma a instituciones educativas o departamentos de RRHH que quieran evaluar la verdadera capacidad de resolución de los candidatos sin intervención de IA.

4. Conclusión
CÓRTEX no es una app de hábitos ni un juego. Es una herramienta de diagnóstico y entrenamiento para la era post-IA. Su desarrollo demuestra capacidad de análisis de tendencias, diseño ético de producto y dominio de tecnologías de integración de APIs y ejecución segura de código.
