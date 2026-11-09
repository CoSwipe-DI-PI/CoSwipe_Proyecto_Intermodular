# Sprint 2

## 2.1. Sector profesional y perfil de usuario

### 2.1.1. Tabla descriptiva del sector y sus características organizativas.

Nuestra App se amolda a los sectores de apps móviles, películas/streaming y videojuegos.
Estudio de la organización de los sectores , tendencias de digtalización y necesidades técnologicas:

| Dimensión | Características Organizativas del Sector | Tendencias de Digitalización | Necesidades Tecnológicas |
|---|---|---|---|
| **Apps Utilidad/B2C** | • Equipos pequeños y ágiles: Trabajo en grupos reducidos que lanzan y mejoran la app de forma continua.<br><br>• Dependencia de Plataforma Dominantes: Obligación de cumplir las normas y comisiones de Apple y Google para poder publicar. | • Cero fricción: Entrar sin crear cuenta , con un Pin o un QR .<br><br>• Estrategias Product-Led Growth (PLG): La experiencia de producto actúa como principal motor de adquisición. | • Desarrollo Multiplataforma Eficiente: Necesidad de frameworks híbridos (Flutter, React Native) para minimizar costes de desarrollo entre iOS y Android.<br><br>• Backend en la nube con tiempo real: Microservicios en la nube (AWS/GCP/Firebase). |
| **Películas y Streaming** | • Concentración Corporativa y Licenciamiento: El mercado es un oligopolio de medios (Hollywood Studios, Tech Giants).<br><br>• Equipos globales: Divisiones centradas en gestionar licencias de catálogo, crear producciones y adaptar los vídeos para todo el mundo. | • Modelos Híbridos Monetizados: Integración de publicidad insertada en planes de bajo coste (AVOD/FAST).<br><br>• Globalización Inmediata del Contenido: Digitalización y automatización de procesos de localización, subtitulado por IA y doblaje para lanzamientos mundiales simultáneos. | • Conexión a catálogos (APIs): Integración con servicios externos para obtener automáticamente portadas, sinopsis y plataformas donde ver cada título.<br><br>• Algoritmos de Recomendación Avanzados: Motores de filtrado colaborativo/basado en contenido para mitigar la "fatiga de elección" del usuario. |
| **Videojuegos** | • Grandes estudios AAAcon jerarquías complejas y gran presupuesto.<br><br>• Pequeños estudios independientes (Indies), a menudo dependientes de Publishers para la distribución. | • Democratización de Motores de Desarrollo: (Unity, Unreal Engine) que aceleran los tiempos de desarrollo e integraciones.<br><br>• Centralización en Tiendas Digitales y Cloud Gaming: Abandono del formato físico en favor de distribuidores digitales (Steam, Epic, Xbox Store, PlayStation Network) y servicios de juegos en la nube. | • Bases de Datos de Compatibilidad y Cross-Platform: Necesidad de APIs unificadas para consultar compatibilidad de plataformas (cross-play), requerimientos de hardware y modos multijugador (co-op).<br><br>• Sistemas de Matchmaking y Networking Social: Infraestructura de servidores con baja latencia para gestionar sesiones multijugador y lobbies grupales. |

### 2.1.2. Fichas Buyer Persona/User Persona

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/ecf9c4ed-949c-4898-8172-ec038873d21e" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/179d647c-4a51-4308-b2a2-91855368a38a" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/138b4096-9ea7-44a3-a90f-ccbc20f20249" />

---

## 2.2. Análisis de la Necesidad

El análisis de la necesidad argumenta y justifica la inversión de recursos técnicos y humanos en el desarrollo de la aplicación CoSwipe, detallando la ineficiencia operativa del modelo tradicional de elección grupal y formalizando la propuesta de valor respaldada en fundamentos teóricos de interacción persona-computadora (HCI).

### 2.2.1. Diagnóstico de la Situación de Partida (As-Is)

En la actualidad, la selección conjunta de contenidos de entretenimiento (películas, series de televisión o videojuegos) en grupos de amigos, compañeros de piso o parejas se realiza mediante un proceso completamente artesanal, desestructurado y analógico/manual:

1. **Búsqueda e Inspección Individual Dispersa:** Cada miembro del grupo consulta de forma aislada e independiente sus propias aplicaciones de streaming (Netflix, Prime Video, HBO Max, Disney+) o plataformas de videojuegos (Steam, PlayStation Network, Epic Games Store). Esto implica saltar continuamente entre múltiples aplicaciones con interfaces y sistemas de navegación heterogéneos.

2. **Coordinación e Intercambio Informal:** Las propuestas se transmiten mediante captura de pantalla, enlaces web sueltos o notas de voz compartidas a través de canales de mensajería instantánea (WhatsApp) o servidores de voz (Discord).

3. **Debate y Evaluación Discontinua:** El grupo intenta negociar verbalmente o mediante texto sin una estructura de votación formal. No existe visibilidad compartida del catálogo total disponible ni se dispone de filtros previos adaptados a los gustos específicos de los participantes en tiempo real.

4. **Iteración Excesiva y Frustración:** El proceso se vuelve un bucle cansado. Como no se llega a un acuerdo, se van rechazando opciones una y otra vez sin recordar en cuáles sí se había coincidido. Esto suele acabar con el grupo rindiéndose sin ver nada o aceptando la propuesta de la persona más insistente por puro cansancio.

### 2.2.2. Problemas y Consecuencias Identificadas

El diagnóstico del escenario As-Is pone de manifiesto deficiencias críticas en la experiencia de usuario (UX):

- **Pérdida Neta de Tiempo Operativo:** El tiempo promedio invertido en alcanzar un acuerdo es de 32,5 minutos por sesión (dato validado empíricamente mediante entrevistas con la metodología Mom Test). Este retraso reduce sustancialmente el tiempo efectivo dedicado al ocio conjunto.

- **Problema de los Catálogos Infinitos:** La inmensa cantidad de opciones repartidas en decenas de plataformas provoca un bloqueo mental (parálisis por elección), haciendo que buscar sea abrumador y consumir el contenido pase a segundo plano.

- **Sesgo de la Voz Dominante y Monopolio de Elección:** Sin un mecanismo de votación anónimo y democrático, las decisiones suelen ser monopolizadas por la persona propietaria de la cuenta o por el perfil más ruidoso del grupo, generando insatisfacción en el resto.

- **Alta Fricción de Entrada:** Las pocas herramientas existentes en el mercado obligan a todos los participantes a crear cuentas de usuario, verificar correos electrónicos o instalar aplicaciones pesadas, provocando el rechazo directo de aquellos usuarios que solo buscan unirse a una votación puntual de 2 minutos.

### 2.2.3. Propuesta de Valor y Situación Deseada (To-Be)

CoSwipe transforma radicalmente este flujo mediante una arquitectura multiplataforma (Desktop Java Swing / FlatLaf Dark y cliente ligero web/móvil) orientada al concepto de Zero-Friction Group Decision:

- **Acceso Instantáneo sin Registro:** El anfitrión crea la sala y los participantes se unen en menos de 5 segundos escaneando un código QR o introduciendo un PIN de 6 dígitos, sin necesidad de registro previo ni recolección de datos personales.

- **Catálogo Unificado Multi-Categoría (Cine, Series y Videojuegos):** La aplicación consolida en una única interfaz el catálogo dinámico de contenido, permitiendo filtrar de forma previa por plataformas activas en el grupo (Netflix, Steam, etc.) y géneros.

- **Mesa de Votación Gestual Síncrona (Swipe Deck):** Los usuarios evalúan las tarjetas de contenido de forma independiente y simultánea mediante gestos de deslizamiento o teclas de acceso directo (PASS con tecla A/← y LIKE con tecla D/→).

- **Detección Automática de Coincidencia Unánime (Match):** El sistema procesa los votos en tiempo real. Al detectar el primer contenido con el 100% de aprobación del grupo, interrumpe la votación y presenta la tarjeta ganadora con acceso directo a la plataforma de reproducción o juego.

### 2.2.4. Aportación Documental

#### 2.2.4.1. Fundamentación Teórica e Investigación

El diseño de CoSwipe se articula sobre tres pilares teóricos consolidados en la literatura de Interacción Persona-Computadora (HCI) y la Psicología Cognitiva:

1. **Ley de Hick-Hyman (T=b · log_2(n + 1)) :** Establece que el tiempo (T) requerido para tomar una decisión es una función logarítmica del número de alternativas presentes (n). Al dividir el catálogo infinito en elecciones binarias consecutivas (LIKE / PASS), CoSwipe reduce n a 2 opciones por tarjeta, minimizando el tiempo de respuesta a menos de 3 segundos por elemento.

2. **La Paradoja de la Elección (Barry Schwartz):** Demuestra que aumentar desproporcionadamente las opciones no genera libertad, sino parálisis y frustración. CoSwipe aplica un filtrado previo por plataformas y géneros para acotar el mazo de decisiones a un subconjunto relevante y manejable.

3. **Principios de Usabilidad "Zero-Friction" (Steve Krug):** En su máxima "Don't Make Me Think", Krug defiende la eliminación de barreras cognitivas y burocráticas. Eliminar el formulario de registro e inicio de sesión para los participantes secundarios erradica la tasa de abandono inicial (churn rate).

#### 2.2.4.2. Diagrama Conceptual: Flujo Actual (As-Is) vs. Flujo Propuesto (To-Be)

##### Flujo Actual (As-Is) - Proceso Disperso y No Estructurado

| Rol / Usuario | Acciones Realizadas | Resultado / Problema |
|---|---|---|
| **Usuario 1** | Abre Netflix/Steam, busca títulos manualmente y envía enlaces por WhatsApp. | Aportación dispersa e informal. |
| **Usuario 2** | Abre Prime Video, descarta la propuesta del Usuario 1 y sugiere otra. | Falta de consenso y desorden. |
| **Usuario 3** | Se pierde entre mensajes o no responde; inicia discusión verbal en Discord. | Saturación y falta de visibilidad. |
| **Impacto Global** | Parálisis por elección, pérdida media de 32,5 min y frustración. | Proceso abandonado o impuesto por agotamiento. |

##### Flujo Propuesto con CoSwipe (To-Be) - Proceso Síncrono y Dirigido

| Fase | Acción en CoSwipe | Beneficio / Solución |
|---|---|---|
| **1. Creación de Sala** | Anfitrión selecciona filtros (Streaming/Juegos) y genera PIN/QR. | Configuración rápida y acotada. |
| **2. Acceso Cero Fricción** | Invitados escanean QR o introducen PIN (Acceso en < 5s sin registro). | Entrada inmediata sin barreras. |
| **3. Votación Síncrona** | Votación individual en Mazo Síncrono (Swipe PASS/LIKE o teclas A/D). | Decisión binaria y democrática. |
| **Resultado Consenso** | MATCH unánime alcanzado en < 3 minutos con enlace directo. | Redirección inmediata a la plataforma elegida. |

<img width="3600" height="2140" alt="image" src="https://github.com/user-attachments/assets/761d4834-6ffb-4be4-a821-10c349d94a1d" />


#### 2.2.4.3. Listado Justificado de Requisitos Funcionales y Operativos

##### Requisitos Funcionales (RF)

- **RF-01: Gestión de Salas Cero Fricción:** El sistema debe permitir la creación de salas de votación y el acceso a las mismas mediante un código alfanumérico de 6 dígitos o escaneo de código QR, sin exigir autenticación de usuario.
  - *Justificación:* Elimina la barrera de entrada para usuarios ocasionales, garantizando la incorporación en menos de 5 segundos.

- **RF-02: Filtro Dinámico de Catálogo Multi-Sector:** La aplicación debe permitir acotar las tarjetas de contenido combinando la categoría (Películas, Series, Videojuegos), plataformas activas (Netflix, Steam, etc.) y géneros.
  - *Justificación:* Cumple con la Ley de Hick al reducir el universo de alternativas únicamente a los medios a los que el grupo tiene acceso real.

- **RF-03: Mazo de Votación Interactiva y Accesible:** La interfaz debe presentar fichas de contenido individuales evaluables mediante interacción gestual (PASS/LIKE) o atajos de teclado (A/D, ←/→).
  - *Justificación:* Ofrece una vía de decisión binaria rápida y garantiza la operatividad completa por teclado para usuarios con movilidad reducida (WCAG 2.1 AA).

- **RF-04: Motor de Consenso en Tiempo Real:** El sistema debe procesar los votos en segundo plano y disparar de forma síncrona la pantalla de resultado unánime (Match) en cuanto todos los miembros activos coincidan positivamente en una opción.
  - *Justificación:* Evita seguir evaluando opciones una vez alcanzado el objetivo de la sesión.

##### Requisitos Operativos (RO)

- **RO-01: Accesibilidad Universal (Norma UNE-EN 301549):** La interfaz gráfica debe cumplir con el nivel AA de las WCAG 2.1, ofreciendo navegación por tabulación ordenada (Tab), foco visual de alto contraste (#7C3AED) y soporte para lectores de pantalla.
  - *Justificación:* Garantiza el cumplimiento del marco legal europeo para software accesible.

- **RO-02: Homogeneidad Visual y Regla 60-30-10:** Toda la interfaz debe maquetarse bajo el tema oscuro FlatLaf Dark, utilizando un contraste de color estricto (#0D0E12 Fondo 60%, #1A1C23 Superficies 30%, #7C3AED Acento 10%).
  - *Justificación:* Asegura la legibilidad, reduce la fatiga visual en entornos de ocio nocturno y mantiene la identidad corporativa de la aplicación.

---

## 2.3. Estudio de Soluciones Existentes

El estudio de soluciones existentes mediante análisis comparativo (benchmarking) evalúa las alternativas comerciales y de código abierto presentes en el mercado, argumentando las ventajas competitivas de CoSwipe.

### 2.3.1. Identificación de Software Competidor

Se han seleccionado tres soluciones reales del mercado que abordan de forma parcial el problema de la elección de contenido o la toma de decisiones grupales:

1. **Reelgood / JustWatch (Agregadores de Streaming):** Aplicaciones comerciales orientadas a la localización de películas y series en catálogos de streaming. Permiten consultar dónde ver cada título y gestionar listas de seguimiento personales.

2. **Taste / Likewise (Motores de Recomendación):** Soluciones comerciales basadas en algoritmos de Inteligencia Artificial que sugieren contenidos de cine y televisión según el perfil de preferencias guardado individualmente por el usuario.

3. **StrawPoll / Encuestas de WhatsApp (Herramientas de Votación Genéricas):** Plataformas web o utilidades integradas en mensajería que permiten crear listas de opciones en formato texto para votación por mayoría simple.

### 2.3.2. Análisis Comparativo

- **Usabilidad y Accesibilidad:** Reelgood y Taste cuentan con interfaces modernas pero saturadas de información visual que entorpecen la decisión rápida. Ninguna de estas plataformas soporta navegación adaptada por teclado bajo normas de accesibilidad (WCAG 2.1). Las encuestas de StrawPoll son accesibles pero carecen de riqueza visual (sin portadas, imágenes ni metadatos de las plataformas).

- **Capacidad Multiplataforma:** JustWatch y Reelgood ofrecen versatilidad en entornos móviles y web, pero sus clientes de escritorio son inexistentes o simples envoltorios web (WebWrappers) con alto consumo de memoria RAM. StrawPoll opera exclusivamente vía navegador web.

- **Fricción de Entrada y Registro:** Tanto Taste como Reelgood exigen la creación obligatoria de una cuenta de usuario (correo, contraseña o Social Login) antes de acceder a cualquier función de recomendación.

- **Orientación al Trabajo Grupal Síncrono:** Ninguna de las herramientas analizadas permite la votación síncrona en tiempo real con detección de unanimidad. JustWatch permite compartir listas estáticas, pero no dispone de un mazo interactivo de votación por deslizamiento.

- **Alcance de Catálogos:** Las soluciones existentes se enfocan de manera exclusiva en el cine y la televisión (SVoD), excluyendo por completo la industria de los videojuegos (PC, consolas).

### 2.3.3. Aportación Documental

#### 2.3.3.1. Matriz Comparativa de Mercado

<img width="649" height="755" alt="image" src="https://github.com/user-attachments/assets/aa0fff2d-5e6f-4add-9340-9a24ef182602" />

<img width="3600" height="2480" alt="image" src="https://github.com/user-attachments/assets/8e927278-c437-4a07-a518-27637c2e9be7" />

#### 2.3.3.2. Justificación de la Propuesta de Valor y Ventaja Competitiva

La ventaja competitiva fundamental de CoSwipe radica en la combinación de dos pilares innovadores y diferenciadores: la filosofía Zero-Friction y la integración pionera del catálogo de videojuegos junto al cine y las series. Mientras que la competencia exige registros obligatorios y se limita exclusivamente a plataformas audiovisuales, CoSwipe elimina completamente las barreras de entrada (acceso en menos de 5 segundos mediante PIN o QR) e introduce los videojuegos como una opción de decisión de primer nivel. Esto, sumado a un mazo de votación gestual accesible (operable al 100% por teclado bajo la norma UNE-EN 301549) y un algoritmo de consenso en tiempo real (Match), sitúa a CoSwipe como la solución más ágil y completa del mercado para la elección de ocio en grupo.

---

## 2.4. Partes Interesadas (Stakeholders)

Un Stakeholder es cualquier persona, grupo u organización que puede afectar a la App o verse afectado por él.
Nuestra app entra en el mundo de la tecnología de consumo y el ocio digital (Consumer Tech & B2C Entertainment(Business to Consumer)), donde cada vez hay más plataformas de streaming y cuesta más ponerse de acuerdo sobre qué ver en grupo. Por eso, los grupos de interés van desde quienes desarrollamos y mantenemos la app hasta quienes la usan o pueden aprovecharla.

- **Internos**: Equipo de desarrollo, tutor y mantenimiento de la app / host.
- **Externos**: Usuarios (anfitriones, participantes y usuario final), Plataformas de streaming(Netflix, Prime Video, etc.), Proveedores de datos(TMDB, IGDB / Twitch) e Proveedor cloud(Google).

### Matriz interesados (Poder vs Interés)

| Rol / Grupo | Interno / Externo | Expectativas | Influencia (Poder) | Interés | Estrategia comunicación recomendada |
|---|---|---|---|---|---|
| **Equipo de desarrollo** (Lucía, Felipe, Raúl, Sergio) | Interno | Sacar el proyecto adelante en plazo, con buen código y una memoria completa. Que el reparto de tareas sea justo. | Alto | Alto | **Involucrar**. Daily, Sprint Planning, Review y Retrospective. Tablero de tareas compartido y chat del grupo. |
| **Tutor** | Interno | Evaluar el proyecto intermodular y las entregas de cada Sprint. Que se cumplan los requisitos y se entregue a tiempo. | Alto | Alto | **Involucrar**. Entrega al final de cada Sprint y correo para dudas. |
| **Usuarios** (anfitriones y participantes, de 18 a 31 años) | Externo | Unirse a la sala en segundos sin registro, votar con swipe y decidir en menos de 3 minutos. App gratuita, rápida y sin fricción; que sus datos no se usen sin su consentimiento; que las recomendaciones sean relevantes. | Medio | Alto | **Involucrar**. App fácil de entender, mensajes claros, encuestas rápidas tras usarla, política de privacidad clara y canal de feedback dentro de la app. |
| **Plataformas de streaming** (Netflix, Prime Video, etc.) | Externo | Recibir tráfico hacia sus catálogos. Posibles socios de afiliación. | Medio | Bajo | **Informar**. Presentar el proyecto y proponer colaboración cuando haya una versión estable. |
| **Proveedores de datos** (TMDB, IGDB / Twitch) | Externo | Que se respeten sus términos de uso, límites de peticiones y requisitos de atribución. Que la app haga un uso razonable de sus datos. | Alto | Bajo | **Informar**. Revisar sus condiciones y cambios de versión, y tener un plan B si cambian los términos. |
| **Proveedor cloud** (Google) | Externo | Que se use el servicio dentro de los límites del plan contratado y bajo sus condiciones de uso. | Alto | Bajo | **Informar**. Revisar avisos y cambios de condiciones del servicio. |


<img width="1265" height="827" alt="Image" src="https://github.com/user-attachments/assets/fd95e97a-9063-4909-aa14-cac8cb7482df" />





---

## 2.5. Estudio de viabilidad técnica

### 2.5.1. Pila tecnológica (Tech Stack)

#### Tecnologías propuestas

| Tecnología | Función | Justificación |
|---|---|---|
| **Kotlin** | Lenguaje de programación. | Es el lenguaje elegido para desarrollar la aplicación. |
| **Java Swing** | Desarrollo de la interfaz gráfica de escritorio. | Permitirá crear la interfaz de escritorio de la aplicación utilizando componentes gráficos. |
| **FlatLaf Dark** | Apariencia visual de la interfaz. | Se utilizará para aplicar un diseño oscuro y uniforme a la interfaz gráfica. |
| **Firebase** | Cloud Firestore[1] | Será la base de datos principal. Guardará las salas, los participantes, las tarjetas y los votos, y permitirá sincronizar los cambios entre usuarios. |
| **APIs** | TMDB[2] e IGDB[3] | TMDB permitirá consultar información de películas y series para mostrarla en las tarjetas. IGDB permitirá consultar información de videojuegos para mostrarla en las tarjetas. |
| **Jackson / Gson** | Procesamiento de datos JSON. | Se utilizarán para procesar las respuestas JSON recibidas de las APIs y obtener la información necesaria. |
| **InputMap / ActionMap** | Accesibilidad mediante teclado. | Permitirán configurar los atajos y las acciones del teclado para facilitar la navegación y el uso de la aplicación. |
| **Visual Studio Code o Android Studio** | Entorno de desarrollo. | Permiten escribir, ejecutar, depurar y probar el código desarrollado para la aplicación. |
| **GitHub** | Control de versiones. | Facilita el trabajo colaborativo, la asignación de tareas, el seguimiento de los cambios y la integración del código de los cuatro integrantes. |

#### Arquitectura general

CoSwipe se organizará en tres partes principales:

- **Cliente:** aplicación móvil y versión web desarrolladas con Kotlin, encargadas de mostrar las tarjetas, recoger los votos y presentar los resultados. Para la interfaz de escritorio se utilizará Java Swing junto con FlatLaf Dark.

- **Servicios de datos:** sistema encargado de almacenar la información de las salas y sincronizar los votos de los participantes.

- **APIs externas:** TMDB e IGDB proporcionarán los datos necesarios para mostrar películas, series y videojuegos.

#### Referencias

- [1] Cloud Firestore: base de datos NoSQL en la nube - https://firebase.google.com/docs/firestore
- [2] TMDB: API con información de películas y series - https://www.themoviedb.org/?language=es
- [3] IGDB: API con información de videojuegos - https://www.igdb.com/
- [4] FlatLaf: librería para la apariencia visual de aplicaciones Java Swing - https://www.formdev.com/flatlaf/
- [5] Jackson: librería para procesar datos JSON - https://github.com/FasterXML/jackson
- [6] Gson: librería para procesar datos JSON - https://github.com/google/gson
- [7] WCAG 2.1: pautas de accesibilidad para el contenido web - https://www.w3.org/TR/WCAG21/

---

### 2.5.2. Requisitos de hardware y despliegue

#### Requisitos de los equipos de desarrollo

| Característica | Requisitos mínimos | Requisitos recomendados |
|---|---|---|
| **Sistema operativo** | Windows 10 de 64 bits | Windows 11 de 64 bits |
| **Memoria RAM** | 16 GB | 32 GB |
| **Procesador** | Intel Core i5-8400 o AMD Ryzen 3 1200 | Intel Core i5-12400 o AMD Ryzen 5 5600 |
| **Almacenamiento** | SSD con 30 GB libres | SSD con 100 GB libres |
| **Tarjeta gráfica** | NVIDIA GeForce GTX 1050 de 4 GB | NVIDIA GeForce RTX 2060 de 8 GB |
| **Pantalla** | 1280 × 800 píxeles | 1920 × 1080 píxeles |
| **Conectividad** | Conexión a Internet | Conexión estable a Internet |

#### Requisitos de los dispositivos cliente

##### Aplicación móvil Android

| Característica | Requisitos mínimos | Requisitos recomendados |
|---|---|---|
| **Sistema operativo** | Android 10 | Android 12 o superior |
| **Memoria RAM** | 2 GB | 4 GB |
| **Procesador** | ARM de 64 bits compatible con Android 10 | Qualcomm Snapdragon 680 o equivalente |
| **Almacenamiento libre** | 100 MB | 200 MB |
| **Pantalla** | 720 × 1280 píxeles | 1080 × 2400 píxeles |
| **Tarjeta gráfica** | GPU integrada compatible con Android | GPU integrada compatible con OpenGL ES 3.0 |
| **Conectividad** | Wi-Fi o datos móviles | Wi-Fi o datos móviles estables |

##### Aplicación web

| Característica | Requisitos mínimos | Requisitos recomendados |
|---|---|---|
| **Sistema operativo** | Windows 10 de 64 bits | Windows 11 de 64 bits o sistema equivalente actualizado |
| **Memoria RAM** | 4 GB | 8 GB |
| **Procesador** | Intel Core i3-8100 | Intel Core i5-12400 |
| **Navegador** | Chrome, Edge, Firefox o Safari con una versión compatible | Última versión estable de Chrome, Edge, Firefox o Safari |
| **Pantalla** | 1280 × 720 píxeles | 1920 × 1080 píxeles |
| **Tarjeta gráfica** | Gráficos integrados compatibles con el navegador | Gráficos integrados con aceleración por hardware |
| **Almacenamiento libre** | 100 MB para caché y datos temporales | 500 MB para caché y datos temporales |
| **Conectividad** | Conexión a Internet | Conexión estable a Internet |

---

### 2.5.3. Curva de aprendizaje y madurez técnica

El equipo cuenta con conocimientos previos de Kotlin, Visual Studio Code y Android Studio, ya que estas tecnologías y herramientas se trabajan en clase. Por tanto, no será necesario dedicar tiempo adicional a aprenderlas desde cero.

#### Tiempo estimado de aprendizaje

| Tecnología o herramienta | Situación del equipo | Tiempo estimado de aprendizaje |
|---|---|---|
| **Kotlin** | Se trabaja en clase. | Sin formación inicial prevista, aunque seguramente hará falta dedicarle tiempo. |
| **Android Studio** | Se utiliza en clase. | 0 horas de autoformación inicial. |
| **Cloud Firestore** | Será necesario aprender a configurar la base de datos, almacenar la información de las salas y sincronizar los votos entre usuarios. | 8-12 horas |
| **API de TMDB** | Será necesario aprender a realizar peticiones y procesar las respuestas JSON, ya que envía la información en ese formato, para mostrar películas y series en las tarjetas. | 3-5 horas |
| **API de IGDB** | Será necesario aprender a realizar consultas, gestionar la autenticación de la API y obtener información de videojuegos. | 5-8 horas |
| **FlatLaf Dark** | Será necesario aprender a instalar y configurar la librería para aplicar el diseño oscuro a la interfaz gráfica. | 3-5 horas |
| **Jackson / Gson** | Será necesario aprender a utilizar una de estas librerías para procesar las respuestas JSON de las APIs. | 3-5 horas |
| **InputMap / ActionMap** | Será necesario aprender a configurar las acciones del teclado para facilitar la navegación y el uso de la interfaz. | 4-6 horas |
| **Accesibilidad WCAG 2.1 AA / UNE-EN 301549** | Será necesario conocer las pautas de accesibilidad para comprobar que la aplicación pueda utilizarse correctamente mediante teclado y cumpla los criterios establecidos. | 4-6 horas |

#### Plan de aprendizaje

El aprendizaje se organizará de forma progresiva:

1. **Cloud Firestore:** configurar la base de datos y comprobar que las salas y los votos se sincronizan correctamente entre los participantes.

2. **API de TMDB:** realizar consultas para obtener información de películas y series y mostrarla en las tarjetas.

3. **API de IGDB:** realizar consultas para obtener información de videojuegos e integrarla en la aplicación.

4. **FlatLaf Dark:** instalar y configurar la librería para aplicar una apariencia visual uniforme a la interfaz.

5. **Jackson / Gson:** aprender a procesar las respuestas JSON recibidas de las APIs para extraer los datos necesarios.

6. **Accesibilidad:** trabajar con InputMap y ActionMap para facilitar la navegación mediante teclado y aplicar las pautas WCAG 2.1 AA y UNE-EN 301549.

7. **Despliegue:** publicar la versión web y preparar la aplicación Android para su instalación y prueba.

#### Conclusión de viabilidad técnica

Tras analizar las tecnologías, los requisitos de hardware y los conocimientos del equipo, consideramos que el desarrollo de CoSwipe es técnicamente viable. Las herramientas principales, como Kotlin y Android Studio, ya se trabajan en clase, por lo que el equipo cuenta con una base de conocimientos para comenzar el desarrollo.

Aunque será necesario dedicar tiempo a aprender a utilizar Cloud Firestore, integrar las APIs externas y configurar las herramientas de accesibilidad, son tareas asumibles durante el desarrollo del proyecto. Además, los requisitos de hardware planteados permiten trabajar con los entornos de desarrollo y probar la aplicación en los dispositivos correspondientes.

Por tanto, consideramos que el equipo dispone de los recursos y la capacidad técnica necesarios para desarrollar, integrar y probar CoSwipe, siempre que se complete la formación prevista y se respeten los requisitos establecidos.

---

## 2.6. ESTUDIO DE VIABILIDAD ECONÓMICA

### 2.6.1. Estimación de costes
- **Desarrollo (Personal):** 4 desarrolladores júnior --> 380 h totales (95 h por desarrollador) a 14,73 €/h (11,33 €/h [1] + 30% SS) = **5.597,40 €**
- **Infraestructura y licencias:** Servidor Cloud (60,00 €) [3], licencia Google Play (23,00 €) [2], certificado de firma de código (Code Signing, 85,00 €) y dominio (12,00 €) [4] = **180,00 €**


#### Amortización de Hardware (Lineal)
Para el cálculo de la amortización de los **4 equipos portátiles** del equipo de desarrollo, aplicamos la fórmula lineal estándar de depreciación:


$$\text{Amortización} = \frac{\text{Valor Inicial Conjunto} \, (2.400\text{ €})}{\text{Vida Útil} \, (48\text{ meses})} \times \text{Meses} \, (3) = \mathbf{150,00\text{ €}}$$


#### 2.6.1.1. Costes indirectos, mantenimiento y soporte técnico post-despliegue
- **Suministros:** Consumos proporcionales de electricidad y conectividad a la red durante la fase de desarrollo = **50,00 €**
- **Previsión de mantenimiento y soporte técnico post-despliegue:** Bolsa de 6,8 horas de soporte técnico a 14,73 €/h para resolución de incidencias iniciales = **100,00 €**


#### Presupuesto desglosado


| Partida | Coste (€) |
| :--- | ---: |
| **Personal** (4 devs. x 95 h) [1] | 5.597,40 € |
| **Hardware** (Amortización de 4 equipos) | 150,00 € |
| **Software / Servicios** (Cloud [3], Dominio [4], Play Console [2] y Code Signing) | 180,00 € |
| **Costes indirectos** (Suministros de electricidad y conectividad) | 50,00 € |
| **Mantenimiento y soporte técnico post-despliegue** | 100,00 € |
| **Subtotal** | **6.077,40 €** |
| **Contingencias (10%)** | 607,74 € |
| **TOTAL PROYECTO** | **6.685,14 €** |




### 6.2. Ahorro operativo y ROI (a 24 meses)
- **Ahorro para el usuario:** Reducción del tiempo de elección de 32,5 min a menos de 3 min.
- **Retorno de la Inversión (ROI):** Tomando la nueva inversión total de 6.685,14 € y estimando unos ingresos netos por afiliación B2B de 12.000,00 € en 24 meses:


$$ROI = \frac{\text{Ingresos Netos} - \text{Inversión}}{\text{Inversión}} \times 100 = \frac{12.000,00 - 6.685,14}{6.685,14} \times 100 = \mathbf{79,50\%}$$


- **Plazo de recuperación (Payback):** Estimando un flujo de caja constante de ~500 €/mes, alcanzamos el punto de equilibrio en **13,37 meses**, demostrando la viabilidad a medio plazo del proyecto en equipo.

## Referencias

[1] "Career Programador Junior Salaries. Accedido el 21 de octubre de 2026. [En línea]. Disponible: https://es.indeed.com/career/programador-junior/salaries

[2] "How the Google Play registration fee works - Play Console Help". Google Support. Accedido el 21 de octubre de 2026. [En línea]. Disponible: https://support.google.com/googleplay/android-developer/answer/6112435

[3] "Tarifas de Servidores Cloud VPS y Servidores Privados Virtuales". OVHcloud España. Accedido el 21 de octubre de 2026. [En línea]. Disponible: https://www.ovhcloud.com/es/vps/

[4] "Registro de dominios web y extensiones". IONOS España. Accedido el 21 de octubre de 2026. [En línea]. Disponible: https://www.ionos.es/dominios

---

## 2.7. Estudio de viabilidad legal y normativa

### 2.7.1. Protección de datos personales

La normativa principal que se debe tener en cuenta es el Reglamento General de Protección de Datos (RGPD, Reglamento UE 2016/679) y la Ley Orgánica 3/2018 (LOPDGDD). El RGPD establece que los datos deben tratarse de forma lícita, utilizarse para finalidades concretas y limitarse a la información estrictamente necesaria.

#### Datos personales que utilizará CoSwipe

Aunque la aplicación no exige crear una cuenta, puede manejar información como los nombres o apodos elegidos por los participantes, los identificadores de las salas y los votos realizados. También podrían tratarse datos técnicos, como identificadores de conexión o direcciones IP, dependiendo de la implementación.

Para reducir la información recopilada, se propone utilizar identificadores temporales para los participantes, evitar solicitar correos electrónicos y contraseñas cuando no sean necesarios y limitar los datos guardados en cada sesión. Los votos se utilizarán para calcular las coincidencias entre los miembros del grupo, sin necesidad de crear perfiles permanentes.

#### Base jurídica del tratamiento

De acuerdo con el artículo 6 del RGPD, se establecerán diferentes bases de legitimación dependiendo de la finalidad para la que se utilicen los datos:

- **Consentimiento (artículo 6.1.a):** se utilizará para el tratamiento de los nombres o pseudónimos elegidos por los participantes. El usuario deberá aceptar de forma libre, informada e inequívoca que se utilice esta información para identificarlo dentro de la sala. También podrá retirar su consentimiento.

- **Ejecución del servicio (artículo 6.1.b):** permitirá tratar los datos necesarios para crear y gestionar las salas, identificar a los participantes mediante identificadores temporales, registrar sus votos y calcular las coincidencias. Estos tratamientos son necesarios para ofrecer las funcionalidades principales de CoSwipe.

- **Interés legítimo (artículo 6.1.f):** podrá utilizarse para tratar determinados registros técnicos de conexión, como las direcciones IP, cuando sean necesarios para garantizar la seguridad, detectar accesos no autorizados y prevenir usos indebidos de la aplicación. Para ello, se deberá comprobar que este interés no prevalece sobre los derechos y libertades de los usuarios y limitar la información conservada a la estrictamente necesaria.

Los usuarios deberán recibir información clara sobre los datos que se recopilan, la finalidad de cada tratamiento, su base jurídica y el tiempo durante el que se conservarán.

#### Medidas de seguridad y privacidad

El artículo 25 del RGPD establece la protección de datos desde el diseño y por defecto. En CoSwipe se aplicará mediante las siguientes medidas:

- **Control de accesos:** configurar los permisos para que cada participante solo pueda acceder a la información que necesite y evitar que personas ajenas consulten los votos de una sala.

- **Protección de credenciales:** al no existir registro obligatorio, se evitará almacenar contraseñas propias si no son necesarias. Si se incorporasen en el futuro, se utilizarían algoritmos de hashing adecuados para protegerlas.

- **Eliminación de datos:** al tratarse de salas temporales, se establecerá un periodo de conservación limitado. Los datos de la sesión se eliminarán cuando dejen de ser necesarios, salvo que exista una obligación legítima de conservarlos.

- **Seguridad de la base de datos:** si se utiliza Firebase Cloud Firestore, se configurarán reglas de seguridad para controlar las lecturas y escrituras, evitando que cualquier usuario pueda consultar o modificar libremente los datos de otras salas.

Estas medidas siguen los principios de minimización y protección de datos por defecto establecidos por el RGPD.

### 2.7.2. Propiedad intelectual y licencias

CoSwipe utilizará código desarrollado por el equipo y puede incorporar bibliotecas, herramientas y recursos multimedia de terceros. Cada elemento tiene unas condiciones de uso que deben respetarse, por lo que no basta con que esté disponible gratuitamente en Internet.

#### Licencia del proyecto

Para el código fuente de CoSwipe se debe elegir una licencia que determine cómo pueden utilizarlo, modificarlo y distribuirlo otras personas. Por ejemplo, MIT permite reutilizar el código bajo condiciones relativamente permisivas, mientras que GPL establece obligaciones de copyleft para las obras derivadas que distribuye. Apache 2.0 también permite la reutilización y contempla condiciones específicas sobre patentes.

La decisión dependerá de si el equipo quiere mantener el código privado o permitir su reutilización. Si se pretende distribuir el proyecto como software abierto, MIT podría ser una opción sencilla para un proyecto académico, siempre que se respeten las condiciones aplicables a sus dependencias.

#### Licencias de las tecnologías y recursos externos

El equipo deberá revisar las licencias de las dependencias reales del proyecto. El inventario inicial puede organizarse de esta forma:

| Componente | Aspecto que debe comprobarse |
|---|---|
| **Kotlin** | Condiciones de uso del lenguaje y sus herramientas. |
| **Firebase y Cloud Firestore** | Condiciones del servicio, licencias y posibles costes de uso. |
| **Bibliotecas de Android** | Licencia de cada dependencia incorporada. |
| **Recursos gráficos e iconos** | Permisos de reproducción, modificación y atribución. |
| **APIs de TMDB e IGDB** | Condiciones de acceso, atribución y utilización de sus datos e imágenes. |
| **Código fuente de CoSwipe** | Licencia seleccionada por el equipo. |

La tabla es un inventario inicial de comprobaciones, no una confirmación de que todos los componentes tengan una licencia concreta. Las condiciones deben verificarse en la documentación oficial de cada tecnología y en la versión utilizada. También se debe comprobar que no existan incompatibilidades entre las licencias de las dependencias y la elegida para el proyecto.

En el caso de TMDB e IGDB, será especialmente importante revisar las condiciones de sus APIs y el uso permitido de sus datos, portadas y logotipos. Que una API permita consultar información no significa que todos sus recursos puedan utilizarse sin restricciones.

Por tanto, el objetivo es que CoSwipe pueda desarrollarse y distribuirse respetando los derechos de autor y las condiciones de las herramientas utilizadas.

### 2.7.3. Accesibilidad y otros requisitos aplicables

La accesibilidad busca que las personas puedan utilizar CoSwipe independientemente de sus capacidades. Para orientar su diseño se tendrán en cuenta las pautas WCAG y la norma UNE-EN 301 549, que recoge requisitos de accesibilidad para productos y servicios TIC. La obligación jurídica concreta dependerá de las características del servicio y de la normativa que resulte aplicable.

Las WCAG se organizan en cuatro principios: que el contenido sea perceptible, operable, comprensible y robusto. En CoSwipe, estos principios se pueden aplicar directamente a las tarjetas, los botones, los menús y las pantallas de resultados.

#### Contraste de colores

La aplicación utiliza un modo oscuro, por lo que los textos y los controles deben distinguirse claramente del fondo. Como referencia WCAG 2.1 nivel AA, el texto normal debe alcanzar una relación de contraste mínima de 4,5:1 y el texto grande, de 3:1. Estos valores se pueden comprobar mediante herramientas de análisis de contraste antes de finalizar el diseño.

#### Navegación y controles

En la versión web se deberá mantener un orden lógico de navegación mediante teclado, con un indicador de foco visible. En la aplicación móvil se tendrán en cuenta los mecanismos de accesibilidad de Android y los lectores de pantalla. Además, los botones deberán tener etiquetas comprensibles para que no dependan únicamente de sus iconos.

#### Tamaño de letra y contenido multimedia

Los textos deberán poder ampliarse cuando lo permita la plataforma sin que se pierda información o funcionalidad. Las imágenes que aporten información necesitarán descripciones alternativas cuando corresponda, mientras que los iconos interactivos deberán disponer de nombres accesibles.

#### Alternativas al deslizamiento de tarjetas

Como CoSwipe se basa en el gesto swipe, se deberán ofrecer alternativas para indicar que una película, serie o videojuego gusta o se descarta. Por ejemplo, se pueden incluir botones visibles de aceptación y rechazo. Así, la elección no dependerá exclusivamente de la capacidad de realizar un gesto táctil.

#### Comprobación de la accesibilidad

Durante las pruebas se revisará el contraste, la navegación, el tamaño de los textos, las etiquetas de los controles y el funcionamiento con tecnologías de asistencia. Estas comprobaciones permitirán detectar barreras y corregirlas antes de entregar la aplicación.

En conclusión, aplicar estos criterios desde el diseño permitirá que CoSwipe sea más fácil de utilizar para distintos perfiles de usuarios. La accesibilidad deberá formar parte de las decisiones de diseño y de las pruebas funcionales, no tratarse únicamente como un ajuste visual al final del desarrollo.

### Referencias web

1. Reglamento General de Protección de Datos (RGPD). Unión Europea.  
   https://eur-lex.europa.eu/eli/reg/2016/679/oj

2. Ley Orgánica 3/2018 (LOPDGDD). Boletín Oficial del Estado.  
   https://www.boe.es/eli/es/lo/2018/12/05/3/con

3. Reglas de seguridad de Cloud Firestore. Firebase.  
   https://firebase.google.com/docs/firestore/security/get-started

4. Documentación de las API de TMDB e IGDB. Condiciones de uso y acceso a los datos de películas, series y videojuegos.
   - TMDB: https://developer.themoviedb.org/docs/faq
   - IGDB: https://api-docs.igdb.com/

5. Web Content Accessibility Guidelines (WCAG). W3C. Pautas de accesibilidad para contenidos web.  
   https://www.w3.org/WAI/standards-guidelines/wcag/es

---

## 2.8. Gestión de riesgos del proyecto

| ID | Descripción | Probabilidad | Impacto | Criticidad [1] | Medida de prevención [2] | Plan de contingencia [2] |
|---|---|---|---|---|---|---|
| **R-01** | Curva de aprendizaje en Java Swing y gestión de WebSockets. | Media | Medio | Media | Prototipado previo y uso de componentes maduros en Java. | Simplificar pantallas y componentes complejos de la interfaz. |
| **R-02** | Latencia o fallos en la sincronización en tiempo real de las salas. | Media | Alto | Alta | Arquitectura ligera por eventos y pruebas de carga tempranas. | Ampliar los recursos del servidor en la nube. |
| **R-03** | Incompatibilidades en el empaquetado del archivo ejecutable (.jar/.exe). | Media | Medio | Media | Pruebas de compilación cruzada en diferentes versiones de Java. | Ajustar parámetros de empaquetado nativo (jpackage). |
| **R-04** | Caídas o límites de cuota en APIs externas (TMDB / IGDB). | Baja | Alto | Media | Implementar sistema de caché local para las respuestas. | Aplicar control de peticiones (rate-limiting). |
| **R-05** | Retrasos en la planificación y desviación de entregas del equipo. | Media | Alto | Alta | Seguimiento semanal mediante tablero Kanban. | Priorizar backlog y reducir funciones secundarias. |
| **R-06** | Incumplimiento de la norma de accesibilidad UNE-EN 301549 (WCAG 2.1 AA) en Java Swing. | Media | Medio | Media | Auditoría temprana de contraste de color y navegación por teclado. | Adaptar accesos rápidos de teclado y tooltips en la UI. |

### Referencias

[1] Pirani Risk, "Matriz de riesgos: qué es, ejemplos y cómo crearla fácil", Blog de Gestión de Riesgos, 2025. [En línea]. Disponible: https://www.piranirisk.com/es/blog/matriz-de-riesgos-que-es-ejemplos-y-como-crearla-facil

[2] GlobalSuite Solutions, "¿Qué es la norma ISO 31000 y para qué sirve?", Gestión del Riesgo Empresarial, 2026. [En línea]. Disponible: https://www.globalsuitesolutions.com/es/que-es-la-norma-iso-31000-y-para-que-sirve/
