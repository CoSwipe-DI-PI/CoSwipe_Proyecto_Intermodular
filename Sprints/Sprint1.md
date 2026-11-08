# Repositorio_Proyecto_Intermodular

## 1. INTRODUCCIÓN

## 1.1. Contexto del proyecto

El proyecto CoSwipe se enmarca en el sector productivo de las Tecnologías de la Información y la Comunicación (TIC), concretamente en la industria del Desarrollo de Software y la Distribución Digital de Contenidos de Entretenimiento (Media & Gaming).

Para comprender el entorno donde opera el proyecto, es necesario clasificar las empresas del sector según sus características organizativas y el tipo de producto o servicio que ofrecen:

### Clasificación de empresas del sector

* **Plataformas de Streaming Audiovisual (SVOD - Subscription Video on Demand):**
  * **Ejemplos:** Netflix, Amazon Prime Video, Disney+, Max (HBO).
  * **Tipo de producto/servicio:** Suscripción periódica para acceso ilimitado a catálogos cerrados de películas, series y documentales bajo demanda.
  * **Características organizativas:** Grandes multinacionales tecnológicas con estructuras jerárquicas y divisionales por región geográfica. Operan con modelos intensivos en capital para producción de contenido original y mantenimiento de infraestructura en la nube (CDN).

* **Plataformas de Distribución Digital de Videojuegos:**
  * **Ejemplos:** Valve (Steam), Epic Games Store, Microsoft (Xbox Game Pass), Sony (PlayStation Store).
  * **Tipo de producto/servicio:** Venta directa de licencias digitales de videojuegos, servicios de juego por suscripción y juego en la nube (Cloud Gaming).
  * **Características organizativas:** Empresas del sector tecnológico/videojuegos con estructuras matriciales altamente especializadas en desarrollo de software, gestión de comunidades y licencias con desarrolladores independientes (indies) y publishers AAA.

* **Plataformas de Guía, Agregación e Intermediación de Contenidos (Discovery & Utility Apps):**
  * **Ejemplos:** JustWatch, Reelgood, TasteMates.
  * **Tipo de producto/servicio:** Aplicaciones B2C utilitarias que agregan metadatos de múltiples plataformas para ofrecer motores de búsqueda unificados, guías de disponibilidad regional y sistemas de recomendación.
  * **Características organizativas:** Startups o PyMEs tecnológicas con estructuras organizativas ágiles (Flat / Lean Organization), enfocadas en el desarrollo rápido de producto, analítica de datos (Big Data) y monetización mediante afiliación o publicidad B2B.

---

### Estructura organizativa y funciones departamentales de una empresa tipo del sector

Una empresa representativa del sector de desarrollo de herramientas de agregación y software multimedia presenta la siguiente estructura funcional:

* **Departamento de Producto (UI/UX & Product Management):**
  * **Funciones:** Definir la visión del producto, diseñar los flujos de experiencia de usuario (UX), elaborar prototipos de interfaz (UI), analizar métricas de retención de usuarios y priorizar el mapa de características (roadmap).

* **Departamento de Ingeniería y Desarrollo de Software:**
  * **Funciones:** Construir la arquitectura de software (frontend móvil y backend), implementar APIs de integración con bases de datos de terceros (TMDB, IGDB), gestionar la infraestructura de servidores síncronos en la nube y asegurar la escalabilidad del sistema.

* **Departamento de Marketing y Analítica de Datos (Growth & BI):**
  * **Funciones:** Diseñar estrategias de adquisición y retención de usuarios, analizar patrones de consumo mediante inteligencia de negocio (Business Intelligence) y gestionar la presencia en tiendas de aplicaciones (ASO - App Store Optimization).

* **Departamento de Desarrollo de Negocio y Asuntos Legales:**
  * **Funciones:** Negociar acuerdos de afiliación con las plataformas de streaming, asegurar el cumplimiento normativo de protección de datos (RGPD) y gestionar licencias de propiedad intelectual relativas al uso de marcas y portadas.

---

### Análisis de contexto multinivel (Macro-Meso-Micro)

Para la fundamentación teórica del proyecto, aplicamos un Análisis de Contexto Multinivel (Macro-Meso-Micro) basado en la Teoría de los Sistemas Ecológicos (Bronfenbrenner, 1979). Esta metodología nos permite encuadrar el nacimiento de CoSwipe a través de tres niveles interconectados, desde las macrotendencias globales de consumo e interfaz hasta el escenario de interacción técnica síncrona:

1. **MACRO (Sistemas Globales):** Transición al Streaming y UI/UX
2. **MESO (Entorno Social):** Nuevos Hábitos de Convivencia
3. **MICRO (Interacción Técnica):** Inmediadez y Sincronización
4. **PUNTO DE CONVERGENCIA:** Proyecto CoSwipe

#### 1. Nivel Macro (Macrosistema): Transformación de la Industria Digital y de las Interfaces
En la capa más global e institucional, la última década ha estado definida por dos grandes transformaciones tecnológicas:
* **La consolidación de los modelos de suscripción masiva:** La industria del entretenimiento ha migrado hacia catálogos unificados digitalmente. Servicios audiovisuales como Netflix, Disney+, Prime Video o HBO Max, junto con plataformas de distribución e integración de videojuegos como Steam, Xbox Game Pass y PlayStation Plus, han digitalizado el consumo de contenidos, centralizando miles de títulos en un único dispositivo.
* **La estandarización de las interfaces gestuales (Swipe UI):** En el ámbito del diseño de interacción, la mecánica de tarjetas deslizables (*swiping*) pasó de ser un recurso innovador en aplicaciones de citas (Tinder, 2012) a un patrón de interacción universal consolidado por plataformas de consumo rápido como TikTok. Este paradigma ha redefinido las expectativas visuales y gestuales de los usuarios, priorizando interacciones de bajo esfuerzo cognitivo y respuesta inmediata.

#### 2. Nivel Meso (Mesosistema): Evolución de los Entornos de Socialización y Consumo Compartido
Al descender al nivel de los grupos de referencia y entornos sociales comunitarios (frecuentados por usuarios de la Generación Z y Millennials), se observan dos espacios dominantes de relación:
* **Espacios de convivencia presencial:** Reuniones en el hogar entre parejas o compañeros de piso compartido, donde la interacción con los contenidos se ejecuta de forma colectiva sobre la pantalla principal del hogar (Smart TV o consola).
* **Entornos de convivencia digital:** Servidores y canales de voz virtuales como Discord, que operan como el punto de reunión habitual para comunidades de amigos que buscan consumir partidas de videojuegos o sesiones de cine simultáneas a distancia.

En ambos entornos, la interacción socio-técnica se caracteriza por ser multi-dispositivo y dinámica: los participantes interactúan individualmente desde sus terminales móviles mientras forman parte de la conversación grupal.

#### 3. Nivel Micro (Microsistema): Arquitectura de Interacción Síncrona sin Fricción
En la escala técnica e individual, el diseño de aplicaciones móviles modernas se orienta hacia la eliminación de barreras de uso y la sincronización inmediata:
* **Sincronización de estado en tiempo real:** El avance en las arquitecturas cliente-servidor y la gestión de eventos síncronos permite conectar múltiples dispositivos móviles dentro de una misma sesión con latencias inapreciables.
* **Diseño sin fricción de entrada (Zero-Friction UI):** La tendencia en herramientas utilitarias efímeras prioriza la reducción de pasos previos. El acceso mediante códigos PIN, códigos QR o enlaces directos evita los flujos tradicionales de onboarding y creación de perfiles con correo electrónico, ajustándose a un uso inmediato.

#### 4. Punto de Convergencia: El Nacimiento de CoSwipe
El proyecto CoSwipe se sitúa exactamente en la convergencia de estos tres niveles: adopta la madurez de los catálogos multimedia actuales (nivel Macro), aprovecha la familiaridad del patrón gestual *swipe* y la tecnología de sincronización en tiempo real (nivel Micro) para responder a las necesidades de interacción de los grupos sociales en entornos presenciales y virtuales (nivel Meso).

---

## 1.2. Problema o necesidad detectada

En los encuentros de ocio compartido, ya sea en una reunión presencial en el salón o en un canal de voz de Discord, la tarea de elegir qué contenido ver o a qué videojuego jugar suele convertirse en un proceso lento de navegación por múltiples catálogos que termina por agotar el tiempo libre del grupo.

### Definición de la parálisis por elección

Este bloqueo responde a un fenómeno conocido en la psicología cognitiva como **parálisis por elección** (*choice overload*), el cual ocurre cuando el volumen excesivo de opciones disponibles sobrepasa la capacidad de procesamiento de la mente humana. Lejos de aumentar la satisfacción o dar libertad al usuario, la sobreoferta produce una elevada carga cognitiva y una acusada fatiga de decisión. Ante cientos de títulos al alcance de un clic, las personas entran en un estado de cuestionamiento continuo por temor a tomar una decisión mediocre, lo que posterga la elección, genera dudas en el grupo y reduce significativamente el disfrute de la experiencia final.

---

### Métodos de investigación del problema y resultados

Para comprobar si esta parálisis por elección afectaba de forma real y medible a nuestros usuarios potenciales, aplicamos la metodología de investigación cualitativa conocida como **The Mom Test**, desarrollada por Rob Fitzpatrick. La regla fundamental de este marco radica en no mencionar jamás la idea de la aplicación ni el producto propuesto, sino enfocar las preguntas exclusivamente en comportamientos pasados, hábitos reales y dificultades sufridas por los entrevistados. De esta manera, se evitan respuestas falsas dadas por compromiso, cortesía o promesas de uso futuro que rara vez se cumplen.

Llevamos a cabo 10 entrevistas individuales a personas de entre 18 y 31 años y los resultados confirmaron una presencia masiva del problema: un **90%** de los participantes (9 de cada 10) afirmó haber sufrido discusiones o bloqueos al intentar ponerse de acuerdo, calculándose una pérdida media de **32,5 minutos** por cada intento de elección antes de iniciar la actividad. Esta frustración quedó reflejada en testimonios directos de los usuarios, quienes señalaban que en Discord pueden pasar 20 minutos preguntando a qué jugar hasta que la gente termina saliéndose del canal de voz, que en los pisos compartidos siempre acaba decidiendo la misma persona, o que en pareja se tarda más tiempo viendo los tráilers que la propia película.

Para profundizar en el estado emocional y conductual de los usuarios durante estos momentos de bloqueo, sintetizamos la información obtenida mediante un **Mapa de Empatía** (*Empathy Map*), una herramienta propia del Design Thinking que organiza los hallazgos en torno a lo que el usuario piensa, siente, oye, ve, dice y hace.

A través de esta perspectiva, observamos que el usuario nota constantemente que está perdiendo su tiempo de ocio y siente pereza ante la idea de iniciar otra discusión, por lo que su único deseo es empezar a jugar o ver algo de inmediato. En su entorno escucha con frecuencia comentarios como *"Entrad a voz y decidimos"*, *"A mí me da igual lo que pongáis"* o *"Ese juego a mí no me va"*, mientras observa catálogos infinitos en la televisión o en bibliotecas como Steam, con sus amigos distraídos con el móvil en el sofá o desconectándose de la llamada. Como consecuencia, el usuario navega sin rumbo por los menús y acaba cediendo por mero agotamiento ante la opción que impone el miembro más insistente del grupo.

* **Puntos de dolor identificados:**
  * **Catálogos infinitos:** Saturación de opciones en Smart TV y Steam.
  * **Decisión impuesta:** Cansancio que lleva a ceder ante el más insistente.
  * **Fricción de registros:** Rechazo a crear cuentas para salas puntuales.

* **Objetivos del usuario (Deseos de cambio):**
  * **Decisión rápida:** Conclusión de voto en menos de 3 minutos.
  * **Voto democrático:** Algoritmo imparcial donde todos cuentan igual.
  * **Acceso directo:** Entrada por código PIN, QR o enlace sin registro.

---

### Análisis de competencia

Para analizar por qué las herramientas existentes no han resuelto este problema, hemos utilizado la metodología de minería de reseñas (**Review Mining**). Esta técnica consiste en recopilar, analizar y categorizar opiniones negativas (de 1 a 3 estrellas) dejadas por los usuarios en tiendas de aplicaciones como Google Play y App Store. En nuestro caso, extrajimos 100 reseñas de competidores directos e indirectos (TasteMates, Movie Fwd, JustWatch y Reelgood) para identificar los principales puntos de fallo de la competencia:

* **42% — Registro e inicio de sesión obligatorio:** El motivo principal por el que los usuarios borran la aplicación antes de usarla en grupo.
* **28% — Fallos de sincronización:** Desconexiones y errores en el directo de la sala.
* **18% — Ausencia de videojuegos:** Limitación exclusiva a cine y series.
* **12% — Restricciones regionales:** Contenido mostrado no disponible en la zona geográfica.

---

### Síntesis de la necesidad detectada

A partir de las carencias del mercado identificadas mediante la minería de reseñas (*Review Mining*) y los datos obtenidos en la investigación cualitativa de campo, se evidencia la necesidad clara de desarrollar una herramienta digital síncrona, imparcial y multiplataforma que:

* Reduzca el tiempo de decisión de más de 30 minutos a menos de 3 minutos.
* Elimine el registro obligatorio (0% fricción) permitiendo unirse mediante código PIN, QR o enlace, resolviendo directamente el principal motivo de rechazo detectado en el análisis de reseñas de la competencia.
* Centralice los catálogos de Cine, Series y Videojuegos en una misma interfaz interactiva.

#### Desde la perspectiva del sector
Esta problemática impacta directamente en la estructura organizativa de las empresas de entretenimiento; mientras los departamentos de Producto y Experiencia de Usuario (UI/UX) detectan altas tasas de abandono cuando la gente se cansa de buscar en los menús, los departamentos de Negocio y Marketing ven reducida la efectividad para dar a conocer sus catálogos. Esta situación abre una clara oportunidad de negocio en el sector de las tecnologías para un modelo utilitario de intermediación B2C (Business to Consumer, enfocado en ofrecer una herramienta directa y práctica al usuario final) y B2B (Business to Business, enfocado en conectar y redirigir clientes hacia las propias plataformas de streaming y tiendas de videojuegos). Este modelo permite capturar tráfico de alta intención de consumo (grupos de personas que ya están reunidas y listas para ver algo o jugar de inmediato). Para dar respuesta a estas demandas, se requiere un proyecto de desarrollo de software utilitario y síncrono (donde todos los móviles conectados se actualizan al mismo tiempo), orientado por características específicas como la creación de salas efímeras sin registro con acceso por PIN (código de 4 dígitos) o QR (código de escaneo rápido con la cámara), el despliegue de un motor de coincidencia (*Match*) en tiempo real, la unificación de catálogos de cine, series y videojuegos, y el diseño de una interfaz gestual Swipe UI (pantalla con tarjetas interactivas que se deslizan a los lados con el dedo) de baja carga mental que permita decidir en menos de 3 minutos.

---

## 1.3. Propuesta de solución

Como respuesta a la parálisis por elección y a las barreras detectadas en las plataformas existentes, se propone el desarrollo de **CoSwipe**, una aplicación móvil multiplataforma orientada a automatizar y gamificar la toma de decisiones grupales de entretenimiento en tiempo real.

CoSwipe transforma un proceso de negociación largo y conflictivo en una interacción ágil, imparcial y divertida, reduciendo el tiempo medio de elección de más de 30 minutos a menos de 3 minutos.

### Flujo de funcionamiento del sistema

El funcionamiento de la aplicación se articula en tres etapas secuenciales diseñadas para eliminar cualquier punto de fricción durante la sesión:

1. **Acceso instantáneo y configuración de la sala (Zero-Friction Onboarding):**
   El anfitrión (*host*) inicia la sesión en cuestión de segundos sin necesidad de crear una cuenta ni introducir credenciales. La aplicación genera una sala virtual asignando un código PIN único de 4 dígitos, un código QR y un enlace directo (*deep link*) listo para compartirse por canales como Discord o WhatsApp. Antes de dar paso a los participantes, el anfitrión ajusta filtros rápidos como el tipo de contenido (Cine, Series o Videojuegos) y las plataformas activas en el grupo (Netflix, Prime Video, Steam, Xbox Game Pass, etc.).

2. **Votación gestual síncrona (Swipe Deck):**
   Los participantes se unen a la sala desde sus propios dispositivos móviles escaneando el código QR o introduciendo el PIN, accediendo de forma anónima e inmediata. Cada integrante recibe una baraja idéntica de tarjetas multimedia limitadas y filtradas. La navegación se basa en la mecánica gestual de deslizamiento:
   * **Deslizar a la derecha (*Swipe Right / Like*):** Indica interés por el título presentado.
   * **Deslizar a la izquierda (*Swipe Left / Pass*):** Descarta la opción.
   
   Las decisiones se procesan de forma individual y privada, protegiendo el voto de cada usuario para evitar la presión de grupo o el sesgo de dominancia.

3. **Algoritmo de coincidencia en tiempo real (Match Engine):**
   A través de un motor de sincronización síncrono, el sistema evalúa los votos de los integrantes en directo. En el momento en que se detecta una coincidencia unánime (todos los miembros de la sala han deslizado a la derecha el mismo título), la interfaz interrumpe la votación y despliega una pantalla interactiva de *Match*. Esta pantalla muestra la opción ganadora de manera destacada e indica la plataforma o servicio exacto donde consumir el contenido de forma inmediata. Si la baraja finaliza sin una unanimidad absoluta, el sistema propone automáticamente la opción con mayor puntuación ponderada.

---

### Pilares clave de la solución

* **Acceso sin registro (0% fricción):** Elimina el principal motivo de rechazo de la competencia (42% en el análisis de reseñas) al no exigir correos ni contraseñas. Unirse a una sala requiere menos de 5 segundos.
* **Catálogo multi-entretenimiento:** Unifica en un mismo sistema cine, series y videojuegos cooperativos/multijugador, adaptándose tanto a reuniones en el salón como a canales de voz en servidores de Discord.
* **Votación a ciegas e imparcial:** Las decisiones son confidenciales mientras se vota, lo que evita el sesgo de dominancia (que decida siempre la misma persona) y elimina la presión social dentro del grupo.
* **Sincronización síncrona en directo:** Un motor en tiempo real evalúa los votos al instante, deteniendo la sesión de forma automatizada en cuanto existe consenso unánime.
* **Diseño optimizado en modo oscuro:** Interfaz gráfica orientada al uso nocturno basada en la regla 60-30-10 (`#0D0E12` fondo, `#1A1C23` tarjetas, `#7C3AED` acento), reduciendo la fatiga visual y priorizando las carátulas e información esencial.

---

## 1.4. Objetivos del proyecto

### 1.4.1. Objetivo general

Desarrollar una aplicación móvil multiplataforma que permita al grupo decidir rápidamente qué películas, series ver o qué videojuegos jugar. El método de decisión será una pantalla con tarjetas que se deslizan (*swipe*) y que se sincroniza en tiempo real entre varios dispositivos conectados a una sala virtual.

El objetivo es evitar la parálisis por elección grupal y que haya desacuerdos. Con esto se quiere reducir el tiempo que el grupo necesita para elegir. La aplicación dará un resultado en base a la tarjeta más elegida. Con esto pretendemos reducir el tiempo de elección de 30 a 3 min aprox.

La app detectará cuando varias tarjetas obtengan el mismo número de me gusta y propondrá más tarjetas para desempatar al grupo. También mostrará en qué plataforma está disponible, para que el grupo pueda jugar o ver de inmediato.

---

### 1.4.2. Objetivos específicos

Para determinar los objetivos específicos usamos la metodología de desarrollo más usada de la industria, la metodología **SCRUM**, que nosotros hemos adaptado a nuestro proyecto de la siguiente manera:

1. **Análisis y Diseño:** Diseñar un prototipo visual de todas las pantallas de la aplicación, apoyándose en un estudio comparativo (*benchmarking*) de aplicaciones similares y en un análisis de la curva de aprendizaje del usuario. Para ello nos apoyaremos en aplicaciones como Figma.
2. **Tecnología:** Seleccionar el lenguaje de desarrollo más adecuado para nosotros (Dart o Kotlin) para hacer la app móvil, usar Swing/Matisse para la de escritorio y aplicar la arquitectura Modelo-Vista-Controlador.
3. **Implementación de la interfaz:** Implementar el algoritmo de coincidencia (*match*) y la funcionalidad de elección (*swipe*).
4. **Datos:** Diseñar la base de datos y analizar qué tipo de SGBD se adapta mejor al proyecto, comparar MongoDB vs MySQL/PostgreSQL en términos de escalabilidad, consultas y facilidad de integración y seleccionarlo.
5. **Servidor:** Comparar tecnologías de backend (Node.js, Spring Boot, Firebase, etc.) según necesidades del proyecto. Escoger API REST a usar para las tarjetas y funcionalidad de salas.
6. **Integración:** Implementar la gestión de salas sincronizadas conectando la aplicación con la base de datos y el servidor.
7. **Pruebas:** Pruebas, corrección de errores y versión final.

---

## 1.5. Alcance del proyecto

Para determinar el alcance funcional del proyecto se ha aplicado la metodología de **Análisis de Requisitos**, la cual ha permitido identificar, clasificar y delimitar con precisión las áreas operativas del sistema, así como las técnicas necesarias para su implementación.

El sistema comprende los siguientes módulos y funcionalidades específicas:

### Módulos y funcionalidades del sistema

1. **Módulo de Gestión de Salas:**
   Este módulo recoge la administración general del ciclo de vida de las salas:
   * **Creación y configuración:** Permite a un usuario (anfitrión) iniciar una nueva sala de decisión y establecer los parámetros iniciales de la sesión.
   * **Cierre de sala:** Gestión de la finalización de la sesión, ya sea por haber alcanzado un consenso (*Match*) o por la decisión voluntaria del anfitrión.
   * **Unión de participantes:** Mecanismo rápido e intuitivo para que los integrantes se unan a una sala a través de dos alternativas:
     * Ingreso manual de un código numérico único (de 4 a 6 dígitos).
     * Escaneo de código QR generado automáticamente por la aplicación al momento de que se cree la sala.

2. **Módulo de Filtros Previos:**
   Permite acotar el catálogo de elementos visualizados según las preferencias colectivas o individuales configuradas antes de iniciar la ronda de selección:
   * **Selección de modo:** Opción para elegir entre la búsqueda de películas o juegos.
   * **Plataformas disponibles:** Filtro por proveedores de streaming de vídeo (para películas) o consolas/plataformas (para juegos) a las que los usuarios tienen acceso.

3. **Módulo de Interacción (Swipe):**
   Constituye el núcleo funcional de la experiencia de usuario dentro de la aplicación:
   * **Interfaz táctil e interactiva:** Diseño centrado en gestos táctiles (*swipe*) para indicar que le gusta o disgusta la opción.
   * **Optimización de carga:** Limitación de cartas por ronda de selección, asegurando un rendimiento fluido y reduciendo el consumo de datos y recursos en el dispositivo móvil.

4. **Sincronización en Tiempo Real:**
   * **Comunicación bidireccional:** Conexión continua entre el servidor central y las aplicaciones móviles conectadas a la misma sala.
   * **Detección instantánea de coincidencias:** Procesamiento en tiempo real de los votos de los integrantes para detectar de forma inmediata cuando existe un consenso (*Match*).

5. **Módulo de Resultados e Información:**
   Encargado de presentar el desenlace de la ronda:
   * **Pantalla de Consenso (Match):** Notificación visual cuando los integrantes coinciden en una elección.
   * **Detalle de disponibilidad:** Muestra la información específica sobre las plataformas exactas donde se puede consumir la película o jugar al título seleccionado.

6. **Compatibilidad y Despliegue Multiplataforma:**
   * **Cobertura de dispositivos:** Desarrollo y despliegue funcional garantizado para dispositivos móviles con sistemas operativos Android e iOS, manteniendo la consistencia de interfaz y comportamiento en ambas plataformas.

7. **Obligaciones fiscales y laborales:**
   * Cumplimiento de los impuestos (IVA, IRPF) y normativa laboral vigente para el equipo de desarrollo.

8. **Prevención de Riesgos Laborales (PRL):**
   * Creación de un plan básico de prevención enfocado en riesgos ergonómicos y visuales por el uso prolongado de ordenadores.

9. **Organización económica y subvenciones:**
   * Estimación de costes (servidores, licencias) y solicitud de subvenciones públicas para nuevas tecnologías.

---

## 1.6. Limitaciones y exclusiones

### Limitaciones

* **Dependencia de APIs de terceros:** La disponibilidad, precisión y actualización del catálogo de películas y videojuegos dependerá directamente de los tiempos de respuesta y límites de consulta (*rate limits*) de las APIs externas (TMDB e IGDB).
* **Conectividad a Internet:** Aunque la sala se denomine "local" por la proximidad física de los usuarios, la sincronización requiere una conexión activa a Internet para la comunicación con la base de datos en la nube.

---

### Exclusiones

* **Reproducción de contenido directo:** La aplicación no actuará como plataforma de reproductor de vídeo ni ejecutor de juegos (*cloud gaming*), su alcance se limita estrictamente a la facilitación de la decisión.
* **Derechos de propiedad intelectual:** Las imágenes, portadas, logotipos y demás elementos identificativos de películas, series y videojuegos estarán sujetos a los derechos de sus respectivos propietarios y a las condiciones de uso establecidas por las fuentes utilizadas.
* **Cambios en la disponibilidad del contenido:** La disponibilidad de películas, series y videojuegos en las diferentes plataformas podrá variar con el tiempo debido a cambios en los catálogos, acuerdos de distribución o condiciones de servicio de dichas plataformas.
* **Red social persistente:** En esta versión del proyecto no se incluirá un sistema de mensajería interna, chat global ni listas de amigos permanentes entre salas.

## 1.7. Estructura de la memoria

| Capítulo | Contenido y enfoque |
|---|---|
| **1. Introducción** | Se presenta el proyecto CoSwipe y su contexto, explicando el problema que se ha detectado, la solución propuesta, los objetivos que se quieren conseguir, el alcance del proyecto y sus principales limitaciones y exclusiones. |
| **2. Análisis del Contexto y Viabilidad** | Se analiza el sector en el que se encuentra el proyecto y los usuarios a los que está dirigido. También se estudian las soluciones existentes, las partes interesadas y la viabilidad técnica, económica y legal de desarrollar CoSwipe, además de los posibles riesgos iniciales. |
| **3. Planificación y Gestión del Proyecto** | Se explica cómo se ha organizado el desarrollo del proyecto utilizando Scrum, incluyendo el reparto de tareas y responsabilidades, los roles del equipo, la planificación del trabajo, los recursos necesarios, el presupuesto, la gestión de riesgos y las herramientas utilizadas para coordinar y realizar el seguimiento del proyecto. |
| **4. Análisis de Requisitos** | Se identifican los distintos tipos de usuarios y se definen las funcionalidades que debe tener CoSwipe, junto con los requisitos no funcionales y las reglas de negocio. También se incluyen los casos de uso o historias de usuario, la prioridad de los requisitos y su relación con las funcionalidades del sistema. |
| **5. Diseño de la Solución** | Se describe cómo se ha planteado técnicamente CoSwipe, incluyendo su arquitectura, los diferentes componentes y módulos, el diseño de la base de datos y de la interfaz de usuario. También se trata el diseño de seguridad y la conexión con las APIs y servicios externos utilizados por la aplicación. |
| **6. Desarrollo e Implementación** | Se detallan las tecnologías, lenguajes y herramientas utilizadas para desarrollar CoSwipe. También se explica cómo se ha organizado el código y cómo se han implementado las principales funcionalidades, la gestión de datos, la interfaz, las integraciones externas y las dependencias del proyecto. |
| **7. Pruebas y Aseguramiento de la Calidad** | Se recoge el proceso utilizado para comprobar que la aplicación funciona correctamente. Se incluyen las diferentes pruebas realizadas, como las pruebas unitarias, de integración y funcionales, además de las comprobaciones de usabilidad, accesibilidad y seguridad. También se muestran los errores encontrados, las soluciones aplicadas y el grado de cumplimiento de los requisitos. |
| **8. Despliegue y Puesta en Producción** | Se explica todo lo relacionado con la preparación de CoSwipe para su ejecución y despliegue. Se incluyen los requisitos de instalación, la configuración necesaria, el proceso de despliegue, las comunicaciones seguras, las copias de seguridad, la monitorización y las tareas de mantenimiento. |
| **9. Manuales de Uso** | Se incluye la documentación necesaria para instalar, utilizar y mantener la aplicación. Este capítulo recoge el manual de instalación, el manual técnico, el manual de usuario y, cuando sea necesario, la guía de administración y las soluciones a problemas habituales. |
| **10. Resultados y Evaluación Final** | Se presentan los resultados obtenidos tras desarrollar CoSwipe y se analiza si se han cumplido los objetivos y requisitos establecidos inicialmente. También se valora el beneficio que aporta la aplicación a los usuarios, las diferencias entre lo planificado y lo realizado, las dificultades encontradas y las competencias utilizadas durante el proyecto. |
| **11. Conclusiones y Líneas Futuras** | Se recogen las principales conclusiones obtenidas durante el desarrollo del proyecto. Además, se plantean posibles mejoras y formas de ampliar o hacer evolucionar CoSwipe en el futuro, junto con una reflexión final sobre los conocimientos y competencias adquiridos. |

*Fecha de entrega: 08/10/2026*

*Enlace presentación:* https://www.canva.com/design/DAHXcNGoiKE/E0Q2G6eIlA9kBFpWO5-rNg/edit?ui=eyJBIjp7fX0

*Enlace prototipo movil:* https://www.figma.com/make/YTBKo1f3rATNGqKR7VOkQe/CoSwipe-Mobile-App-Prototype?code-node-id=0-6&p=f&t=bKVoefMnEjmx2hui-0&fullscreen=1
