
  <img src="https://via.placeholder.com/150?text=Servify+Logo" alt="Logo Servify" width="120">

  <p><strong>Proyecto Personal de Portafolio</strong><br>
  Desarrollo de Aplicaciones Web y Arquitectura de Software</p>

  <br>

<h3><strong>Informe Técnico de Producto</strong></h3>

  <br>

  <p>Producto Digital<br>
  <strong>Servify Web Platform</strong></p>

<br><br>

  <p><strong>Desarrollador / Team Leader</strong></p>

<table style="margin: 0 auto; border-collapse: collapse;">
  <tr>
    <th style="text-align:left; padding: 5px 20px;">Rol</th>
    <th style="text-align:left; padding: 5px 20px;">Apellidos y Nombres</th>
    <th style="text-align:left; padding: 5px 20px;">GitHub</th>
  </tr>
  <tr>
    <td style="padding: 5px 20px;">Full-Stack Developer</td>
    <td style="padding: 5px 20px;">Stephano Moscoso Bejar</td>
    <td style="padding: 5px 20px;"><a href="https://github.com/StephanoDang">@StephanoDang</a></td>
  </tr>
</table>

<br><br>
<p><strong>Lima, Perú</strong></p>
<p><strong>Julio 2026</strong></p>

</div>

---

## Registro de Versiones del Informe

| Versión | Fecha | Autor | Descripción de Modificación |
|---------|-------|-------|-----------------------------|
| 1.0 | 30/07/2026 | Stephano Dang | Creación inicial del documento. Definición del Startup Profile (Misión, Visión y Descripción). |

---

## Contenido

* [Capítulo I: Introducción](#capítulo-i-introducción)
    * [1.1. Startup Profile](#11-startup-profile)
        * [1.1.1. Descripción de la Startup](#111-descripción-de-la-startup)
        * [1.1.2. Perfiles de integrantes del equipo](#112-perfiles-de-integrantes-del-equipo)
    * [1.2. Solution Profile](#12-solution-profile)
        * [1.2.1. Antecedentes y problemática](#121-antecedentes-y-problemática)
        * [1.2.2. Lean UX Process](#122-lean-ux-process)
    * [1.3. Segmentos Objetivo](#13-segmentos-objetivo)
* [Capítulo II: Requirements Elicitation & Analysis](#capítulo-ii-requirements-elicitation--analysis)
* [Capítulo III: Requirements Specification](#capítulo-iii-requirements-specification)
* [Capítulo IV: Product Design](#capítulo-iv-product-design)
* [Capítulo V: Product Implementation, Validation & Deployment](#capítulo-v-product-implementation-validation--deployment)

---

<div style="page-break-after: always;"></div>





# Capítulo I: Introducción

## 1.1. Startup Profile

### 1.1.1. Descripción de la Startup

**Servify** es una startup tecnológica que desarrolla soluciones digitales enfocadas en democratizar la visibilidad online de los trabajadores independientes y emprendedores. A través de su plataforma intuitiva, la aplicación permite a los profesionales crear perfiles personalizados, exhibir galerías visuales de sus proyectos y conectar de manera directa con clientes potenciales. La herramienta digitaliza la oferta de oficios y servicios, transformando el tradicional "boca a boca" en un portafolio digital accesible y profesional para promover negocios más rentables y escalables.

La plataforma está diseñada para atender necesidades específicas de diversos perfiles de usuario. Por un lado, ofrece a los **proveedores de eventos** (decoradores, DJs, servicios de catering, animadores) un espacio especializado para mostrar la calidad de su trabajo sin depender de la complejidad o los algoritmos de las redes sociales; por otro lado, permite a los **trabajadores de oficios técnicos y manuales** (carpinteros, gasfiteros, reposteros) tener una presencia digital formal y confiable. Asimismo, brinda a los **clientes finales** una alternativa segura y centralizada para buscar, comparar mediante reseñas y contactar al talento local adecuado para sus necesidades puntuales.

Con un firme compromiso con la inclusión digital y el empoderamiento económico, **Servify** busca liderar la transformación tecnológica del sector de oficios independientes en el Perú. Al combinar una interfaz amigable orientada a usuarios no nativos digitales con un robusto sistema de perfiles, la startup no solo ayuda a incrementar las oportunidades laborales del talento local, sino que también fomenta una comunidad basada en la transparencia y la confianza profesional, asegurando que cada servicio brindado fortalezca la reputación del trabajador.

**Misión:** Impulsar el crecimiento económico y la formalización digital de los trabajadores independientes mediante soluciones tecnológicas accesibles que aumenten su visibilidad, optimicen la exhibición de su trabajo y faciliten conexiones seguras y directas con clientes que requieran sus servicios.

**Visión:** Ser el marketplace y directorio de oficios de referencia en el Perú y Latinoamérica, liderando la creación de un ecosistema digital inclusivo donde el talento local y las necesidades de los usuarios converjan para generar oportunidades de trabajo justas, transparentes y de alta calidad.


### 1.1.2. Perfiles de integrantes del equipo

Al ser un proyecto de portafolio personal, el desarrollo y arquitectura de la plataforma están a cargo de un único creador que asume todos los roles del ciclo de vida del software.

| Perfil | Datos del Desarrollador | Conocimientos y Habilidades |
| :---: | :--- | :--- |
| <img src="images/stephano.jpeg" width="120" style="border-radius: 8px;"><br>**Full-Stack Developer** | **Nombres y Apellidos:**<br>Angelo Stephano Moscoso Bejar | **Stack Tecnológico:**<br>C++, CSS, HTML, Vue.js, SQL, JS.<br><br>**Aportes al Proyecto:**<br>Encargado del diseño de la arquitectura de datos, desarrollo frontend/backend, maquetación de interfaces responsivas y la implementación de la lógica de negocio. |

## 1.2. Solution Profile

### 1.2.1. Antecedentes y problemática

### Antecedentes
<div style="text-align: justify">

En el mercado laboral actual, la presencia en internet se ha vuelto un factor indispensable para la captación de clientes. Sin embargo, un gran porcentaje de trabajadores independientes, técnicos y profesionales de oficios en el Perú opera en la informalidad digital. A pesar de contar con talento empírico y amplia experiencia, la falta de una plataforma formal, intuitiva y accesible limita su crecimiento comercial, dejándolos en desventaja competitiva frente a agencias o empresas establecidas que sí cuentan con los recursos para mantener sitios web corporativos.

Un caso crítico se observa en el rubro de la organización de eventos privados, como celebraciones de 15 años, bodas o fiestas infantiles. Proveedores de servicios como decoradores, personal de catering, animadores o DJs se ven obligados a depender casi exclusivamente de las recomendaciones tradicionales (el "boca a boca"). Hoy en día se utilizan mucho redes sociales como **TikTok o Instagram** para intentar ganar visibilidad; sin embargo, manejar estas plataformas resulta ser un desafío mayor. Lidiar con los algoritmos, las tendencias y la necesidad de generar contenido viral constante es algo que la gran mayoría de estos trabajadores no logra dominar. Ellos necesitan una herramienta mucho más sencilla y directa que no exija ser un experto creador de contenido, permitiéndoles enfocarse en la ejecución práctica de su verdadero oficio.

Actualmente, la búsqueda y exhibición de estos trabajos es desorganizada. Los profesionales suelen utilizar plataformas genéricas como Facebook Marketplace o se ven en la necesidad de enviar fotografías sueltas por WhatsApp cuando un prospecto solicita ver su portafolio. No existe un ecosistema centralizado donde un decorador, un carpintero o un repostero puedan estructurar un catálogo profesional verificable. La falta de esta herramienta genera un vacío tecnológico que Servify busca llenar, transformando la exhibición informal en un directorio estructurado que conecte el talento local con los clientes de forma directa, profesional y segura, con una curva de aprendizaje mínima.

</div>

### Problemática

<div style="text-align: justify">
Para entender a profundidad la necesidad que impulsa este proyecto, se aplicó la técnica de análisis de las 5W's + 2H's:

### 5W's
### What (¿Cuál es el problema?):
Los trabajadores independientes y proveedores de oficios carecen de un espacio digital especializado e intuitivo para mostrar su portafolio de manera profesional. Esto limita severamente su alcance comercial y crecimiento, mientras que los clientes finales enfrentan dificultades y desconfianza al intentar encontrar talento local verificado sin tener que navegar por redes sociales genéricas y desorganizadas.

### When (¿Cuándo ocurre el problema?):
El problema se evidencia de manera constante, pero se agudiza cuando el profesional intenta conseguir nuevos clientes fuera de su círculo inmediato de referidos, o cuando un cliente necesita organizar un evento (o solucionar un requerimiento técnico) y no cuenta con contactos directos de confianza para realizar el trabajo.

### Where (¿Dónde ocurre el problema?):
En el mercado local de servicios independientes, oficios técnicos y organización de eventos a nivel nacional (Perú), donde la transición hacia la formalización digital aún es deficiente y la oferta de servicios se encuentra dispersa en internet.

### Who (¿A quién o quiénes afecta el problema?):
- **Trabajadores independientes y de oficios:** Decoradores, proveedores de catering, DJs, reposteros, carpinteros y técnicos que pierden oportunidades de contrato por falta de visibilidad online y no dominan la creación de contenido para redes sociales.
- **Clientes finales:** Personas y familias que gastan tiempo valioso buscando profesionales confiables y tienen dificultades para verificar la calidad del trabajo antes de contratar.
- **El desarrollo económico local:** Debido al estancamiento de pequeños emprendedores que no logran escalar sus negocios por la brecha digital.

### Why (¿Por qué sucede el problema?):
Porque desarrollar y mantener una página web propia resulta costoso y técnicamente complejo. Simultáneamente, aunque plataformas como **TikTok e Instagram** están en pleno auge, su manejo exige estrategias de edición, publicación y gestión de comunidades que estos profesionales empíricos no dominan. Ellos necesitan una solución mucho más sencilla y directa para exhibirse. Además, las plataformas de compraventa existentes carecen de filtros diseñados para validar el profesionalismo de los servicios ofrecidos.

### 2H's
### How (¿Cómo aparece el problema?):
El problema se manifiesta a través del estancamiento en la cartera de clientes del trabajador. Constantemente se ven en la necesidad de recurrir a métodos informales, enviando fotos desordenadas por mensajería cuando un potencial cliente pide "ver sus trabajos". Del lado del cliente, este proceso informal genera fricción, se percibe como poco profesional y prolonga innecesariamente la decisión de contratación.

### How Much (¿Cuánto afecta el problema?):
El impacto económico se traduce en una pérdida significativa de contratos potenciales, lo que reduce drásticamente los ingresos mensuales de los emprendedores locales y frena su escalabilidad. Para el cliente, representa un alto costo de oportunidad reflejado en horas invertidas en búsquedas ineficientes y el riesgo financiero de contratar servicios de baja calidad por no contar con un portafolio validado que respalde al trabajador.

</div>

### 1.2.2. Lean UX Process

#### 1.2.2.1. Lean UX Problem Statements

El estado actual de la exhibición de portafolios para trabajadores independientes (proveedores de eventos y oficios) depende del "boca a boca", envío de fotos desordenadas por WhatsApp o del uso de redes sociales complejas (como TikTok o Instagram) que no dominan. Lo que los profesionales necesitan es una forma sencilla y directa de centralizar su trabajo en un perfil profesional sin tener que lidiar con algoritmos ni creación de contenido viral. Hemos observado que la falta de una presencia digital formal limita su crecimiento y les hace perder oportunidades de contrato.

**¿Cómo podríamos diseñar una plataforma accesible que permita a los trabajadores independientes exhibir su portafolio profesionalmente y captar más clientes con una curva de aprendizaje mínima?**

El estado actual de la búsqueda de talento local (decoradores, DJs, técnicos) obliga a los clientes finales a recurrir a plataformas genéricas como Facebook Marketplace o a depender de recomendaciones limitadas de su círculo cercano. Lo que los clientes necesitan es visibilidad sobre la calidad real del trabajo y reseñas confiables para tomar decisiones seguras. Hemos observado que esta fricción genera desconfianza, pérdida de tiempo y el riesgo constante de contratar servicios de baja calidad.

**¿Cómo podríamos ofrecer a los clientes finales un directorio centralizado y confiable que les permita buscar, comparar y contactar rápidamente a profesionales verificados para sus eventos o necesidades del hogar?**

#### 1.2.2.2. Lean UX Assumptions

**Assumptions Worksheet**

- **¿Quién es el usuario?**
  Tenemos dos tipos de usuarios principales: los profesionales de oficios (decoradores, DJs, proveedores de catering, carpinteros, técnicos, etc. que buscan clientes) y los clientes finales (personas o familias que necesitan organizar un evento o solucionar un requerimiento doméstico).

- **¿Dónde encaja nuestro producto en su trabajo o vida?**
  Para el profesional, Servify se integrará como su herramienta principal de ventas y carta de presentación digital. Para el cliente final, funcionará como el directorio de confianza "on-demand" al que acudirán desde su smartphone o computadora cada vez que necesiten cotizar y contratar un servicio específico.

- **¿Qué problemas resuelve nuestro producto?**
  El producto resuelve la informalidad digital del trabajador independiente, la brecha tecnológica que les impide usar redes sociales como canal de ventas eficiente, y la desconfianza/frustración del cliente al buscar talento local verificado.

- **¿Cuándo y cómo es usado nuestro producto?**
  El profesional lo usará para crear/actualizar su galería de trabajos, recibir solicitudes y gestionar contactos. El cliente final lo usará esporádicamente para realizar búsquedas mediante filtros (categoría, ubicación), leer reseñas y presionar un botón de contacto directo.

- **¿Qué características son importantes?**
  Para el segmento de profesionales: creación de perfiles intuitiva, carga rápida de galerías visuales y botón de contacto directo (ej. WhatsApp). Para el segmento de clientes: motor de búsqueda con filtros, sistema de reseñas de 1 a 5 estrellas y validación visual de los proyectos realizados.

- **¿Cómo debe verse nuestro producto y cómo comportarse?**
  Nuestro producto debe transmitir profesionalismo, seguridad y confianza. Su interfaz debe ser extremadamente limpia, visual e intuitiva, asegurando que un profesional no nativo digital pueda configurar su perfil sin fricciones ni confusiones técnicas.

**Business Assumptions:**

- Creemos que los profesionales independientes están dispuestos a pagar una suscripción (mensual o anual) por un perfil "Premium" destacado, siempre que la plataforma les genere un retorno de inversión mediante la captación de nuevos clientes.
- Estas necesidades se pueden resolver mediante un modelo de "Marketplace de Servicios" o directorio digital con un enfoque inicial *freemium* para construir rápidamente una base masiva de proveedores.
- Creemos que los clientes finales prefieren navegar por una plataforma especializada con reseñas y portafolios organizados antes que contactar a desconocidos a través de redes sociales genéricas.
- Nuestro mayor riesgo es el "problema del huevo y la gallina": que los clientes no encuentren suficientes opciones en la plataforma en su etapa inicial, o que los profesionales abandonen sus perfiles si no reciben contactos rápidos.
- Creemos que las alianzas estratégicas con gremios locales, asociaciones de eventos o proveedores mayoristas pueden acelerar la adopción masiva de la plataforma por parte de los trabajadores.

#### 1.2.2.3. Lean UX Hypothesis Statements

- Creemos que si ofrecemos a los trabajadores independientes y proveedores de eventos una plataforma simplificada para crear portafolios profesionales sin requerir conocimientos avanzados en redes sociales, entonces aumentarán su visibilidad online y lograrán captar más clientes. Sabremos que estamos en lo correcto cuando al menos el 30% de los profesionales registrados reciba su primera solicitud de cotización o contacto directo a través de la plataforma durante su primer mes de uso.

- Creemos que si brindamos a los clientes finales un directorio centralizado con galerías visuales y un sistema de reseñas de 1 a 5 estrellas, entonces sentirán mayor seguridad y reducirán el tiempo invertido en buscar talento local confiable. Sabremos que estamos en lo correcto cuando las analíticas muestren que los usuarios completan el flujo desde la búsqueda hasta hacer clic en "Contactar" en menos de 5 minutos, y cuando los servicios contratados mantengan un promedio de calificación superior a 4 estrellas.

- Creemos que si proporcionamos a los profesionales de oficios la opción de adquirir planes de suscripción "Premium" para destacar sus perfiles en los primeros resultados de búsqueda, entonces adoptarán el modelo de pago al percibir un retorno de inversión real. Sabremos que estamos en lo correcto cuando logremos una tasa de conversión de al menos el 15% de usuarios gratuitos a planes de pago dentro de los primeros seis meses de lanzamiento.


#### 1.2.2.4. Lean UX Canvas

<div align="center">
  <img src="images/lean_ux.png" alt="Lean UX Canvas de Servify">
</div>


## 1.3. Segmentos Objetivo

| | Segmento 1: Trabajadores independientes y de oficios | Segmento 2: Clientes finales (Organizadores y hogares) |
| :--- | :--- | :--- |
| **Variables** | Profesionales empíricos, técnicos y proveedores de servicios (decoradores, DJs, catering, mantenimiento). | Personas y familias que requieren contratar servicios para eventos privados o necesidades del hogar. |
| **Geográfica** | Ubicados principalmente en zonas urbanas y suburbanas del Perú (con foco inicial en Lima Metropolitana), donde existe una alta demanda constante de eventos y reparaciones. | Ubicados en zonas urbanas y suburbanas, en distritos con actividad social, familiar y demanda de servicios a domicilio. |
| **Demográfica** | **Edad:** 20-55 años. **Género:** Mixto. **Educación:** Empírica, técnica o superior. **Ingresos:** Variables (dependientes del flujo de contratos). **Ocupación:** Emprendedores de oficios. | **Edad:** 25-55 años. **Género:** Mixto. **Educación:** Secundaria completa o superior. **Ingresos:** Medio a alto. **Estado civil:** Padres de familia, parejas a punto de casarse, solteros independientes. |
| **Psicológica** | Buscan crecimiento económico, formalidad y reconocimiento por su trabajo. Se sienten abrumados por la complejidad de crear contenido viral para redes sociales. Valoran la simplicidad y las herramientas directas que les ahorren tiempo en ventas. | Valoran la confianza, la seguridad y la practicidad. Buscan reducir el riesgo de ser estafados o recibir un mal servicio. Prefieren tomar decisiones racionales basadas en validación visual (fotos/portafolios) y social (reseñas). |
| **Función de comportamiento** | Uso básico o intermedio de smartphones (WhatsApp, Facebook). Adoptan tecnología solo si la curva de aprendizaje es mínima. Se frustran al perder clientes por no tener un catálogo ordenado. Su objetivo principal es cerrar más contratos rápidamente. | Uso frecuente de internet y aplicaciones para resolver necesidades. Se frustran al perder tiempo buscando en grupos desorganizados de Facebook o esperando que les envíen fotos sueltas. Su objetivo es encontrar al proveedor ideal de forma rápida y segura. |



---

<div style="page-break-after: always;"></div>


# Capítulo II: Requirements Elicitation & Analysis

## 2.1. Competidores

### 1. Recomiendame.pe
<div style="text-align: justify">
Recomiendame.pe es un directorio web a nivel nacional enfocado en la búsqueda y recomendación de profesionales y técnicos de diversos oficios. Su plataforma permite a los usuarios buscar servicios específicos y a los trabajadores publicar anuncios básicos sobre lo que hacen. 

En cuanto a costos y modelo de negocio, es una alternativa gratuita o de muy bajo costo; sin embargo, no cuenta con un alto nivel de popularidad, marketing ni adopción masiva por parte de los clientes, lo que limita drásticamente la exposición y el retorno real que obtienen los trabajadores independientes al registrarse allí.
</div>

### 2. Matrimonio.com.pe
<div style="text-align: justify">
Es una de las plataformas web y móviles más grandes en el rubro de eventos sociales en Latinoamérica. Funciona como un directorio súper especializado donde los proveedores de servicios pueden crear un perfil profesional, subir galerías de fotos de alta calidad y recibir reseñas detalladas de sus clientes.

Su modelo de negocio es freemium. Aunque crear un perfil básico es gratuito, la plataforma está altamente saturada, obligando a los profesionales a pagar planes premium costosos para aparecer en los primeros resultados. Además, su principal limitante es que está exclusivamente enfocada en bodas, dejando totalmente por fuera otros eventos privados altamente rentables.
</div>

### 3. Facebook Marketplace y Grupos de Facebook
<div style="text-align: justify">
Aunque no es una plataforma especializada exclusiva para oficios, Facebook (a través de su Marketplace y Grupos locales) es actualmente el principal competidor indirecto, ya que es el ecosistema por defecto al que recurren los trabajadores independientes para intentar captar clientes. Permite subir fotos y colocar descripciones rápidas del servicio ofrecido.

Si bien es una herramienta totalmente gratuita, carece de una estructura profesional para portafolios. Los profesionales se enfrentan a la barrera de los algoritmos de redes sociales, la necesidad constante de "republicar" para no desaparecer, la alta informalidad y la ausencia de un sistema de reseñas centralizado y verificado que brinde seguridad real a los clientes finales frente a posibles estafas.
</div>


### 2.1.1. Análisis Competitivo

<table>
  <tr>
    <th colspan="6">Competitive Analysis Landscape</th>
  </tr>
  <tr>
    <td colspan="2"><b>¿Por qué llevar a cabo este análisis?</b></td>
    <td colspan="4">El objetivo de este análisis es entender cómo los profesionales independientes y técnicos buscan clientes hoy en día, identificar las fallas de las plataformas actuales (desorganización, altos costos, exclusividad) y posicionar a Servify como la alternativa integral, accesible y segura. Esto es vital para encontrar el punto de equilibrio entre la informalidad de las redes sociales y los altos costos de los directorios premium.</td>
  </tr>
  <tr>
    <td colspan="2"></td>
    <td><b>Su startup</b></td>
    <td><b>Competidor 1</b></td>
    <td><b>Competidor 2</b></td>
    <td><b>Competidor 3</b></td>
  </tr>
  <tr>
    <td colspan="2"></td>
    <td><b>Servify</b><br>Perú / Latinoamérica</td>
    <td>
      <b>Recomiendame.pe</b>
      <br>Perú
    </td>
    <td>
      <b>Matrimonio.com.pe</b>
      <br>Latinoamérica
    </td>
    <td>
      <b>Facebook Marketplace</b>
      <br>Global
    </td>
  </tr>

  <tr>
    <td rowspan="2"><b>Perfil</b></td>
    <td><b>Overview</b></td>
    <td>Plataforma digital (web y móvil) diseñada para digitalizar y centralizar portafolios de trabajadores independientes y proveedores de oficios. Permite a los usuarios buscar servicios, ver fotos reales de trabajos anteriores, leer reseñas y contactar directamente por WhatsApp, sin necesidad de dominar redes sociales.</td>
    <td>Directorio web a nivel nacional enfocado en la búsqueda y recomendación de profesionales y técnicos. Permite publicar anuncios textuales y básicos sobre servicios, funcionando como una guía telefónica digital o sección de clasificados modernos.</td>
    <td>Plataforma web y móvil líder en el rubro de eventos sociales (exclusivo bodas). Directorio altamente especializado donde los proveedores crean perfiles premium con galerías de alta calidad, reseñas extensas y herramientas de cotización integradas.</td>
    <td>Sección de compra/venta y grupos comunitarios dentro de la red social Facebook. No es exclusiva para servicios, pero es usada masivamente por profesionales independientes para publicar fotos rápidas y captar clientes en su localidad.</td>
  </tr>
  <tr>
    <td><b>Ventaja competitiva<br>¿Qué valor ofrece a los clientes?</b></td>
    <td>Combina lo mejor de dos mundos: la estructura y formalidad de un portafolio profesional, con la facilidad de uso y contacto directo de una red social. Todo en un entorno validado por reseñas para evitar estafas.</td>
    <td>Enfoque netamente local (Perú) y gratuidad casi total. Es una herramienta sencilla que no exige conocimientos técnicos para crear un anuncio de servicio.</td>
    <td>Prestigio, confianza absoluta y herramientas adicionales (planificadores, foros). Si un proveedor está bien posicionado aquí, garantiza un flujo de clientes con alto poder adquisitivo.</td>
    <td>Tráfico inmenso. El usuario no necesita descargar nada nuevo ni registrarse en otro sitio, ya que utiliza la red social que abre todos los días.</td>
  </tr>

  <tr>
    <td rowspan="2"><b>Perfil de Marketing</b></td>
    <td><b>Mercado objetivo</b></td>
    <td>Trabajadores independientes (20-55 años) del rubro de eventos y oficios técnicos que no dominan algoritmos virales. Clientes finales (familias, organizadores) que buscan servicios rápidos, verificados y sin fricciones.</td>
    <td>Técnicos de oficios tradicionales (gasfiteros, electricistas, albañiles) que buscan un espacio digital básico para dejar su número de contacto en Perú.</td>
    <td>Proveedores de eventos con presupuestos de marketing moderados a altos. Clientes: Parejas comprometidas dispuestas a invertir fuertemente en la celebración de su boda.</td>
    <td>Público general. Cualquier persona con acceso a internet que ofrezca un servicio empírico o que busque soluciones rápidas y económicas en su distrito.</td>
  </tr>
  <tr>
    <td><b>Estrategias de marketing</b></td>
    <td>Marketing digital centrado en la "formalización" del trabajador y el aumento de sus ingresos. Alianzas con gremios locales, mercados y campañas de boca a boca. Crecimiento impulsado por el modelo freemium.</td>
    <td>Posicionamiento SEO local (búsquedas en Google tipo "gasfitero en Lima") y listados gratuitos que atraen tráfico orgánico.</td>
    <td>Fuerte inversión en SEO/SEM, organización de ferias de novios, publicidad tradicional y branding aspiracional muy potente.</td>
    <td>El marketing lo hacen los propios usuarios. Facebook retiene a la audiencia mediante su ecosistema completo (grupos, noticias, chat), haciendo que el Marketplace tenga visitas por defecto.</td>
  </tr>

  <tr>
    <td rowspan="3"><b>Perfil de Producto</b></td>
    <td><b>Productos & Servicios</b></td>
    <td>Perfiles intuitivos, galerías de imágenes de carga rápida, buscador avanzado con filtros, sistema de reseñas de 1 a 5 estrellas y botón de redirección inmediata a WhatsApp para cerrar el trato.</td>
    <td>Fichas de contacto muy básicas con título, descripción del servicio, zona de cobertura y números de teléfono.</td>
    <td>Perfiles premium, cotizador interno, agenda de citas, foros de comunidad y sellos de calidad (premios anuales a los mejores proveedores).</td>
    <td>Publicaciones efímeras en un feed estilo clasificados, interacción en grupos locales e integración directa con Facebook Messenger.</td>
  </tr>
  <tr>
    <td><b>Precios & Costos</b></td>
    <td>Modelo Freemium. Creación de perfil y portafolio 100% gratuito. Planes de suscripción de bajo costo para destacar el perfil en los primeros resultados de búsqueda.</td>
    <td>Gratuito o con opciones de pago de muy bajo costo para mantener el anuncio activo.</td>
    <td>Modelo Freemium altamente agresivo. Aparecer en los resultados útiles requiere pagar planes premium costosos (mensuales o anuales) debido a la saturación del sitio.</td>
    <td>100% gratuito para publicar. Opciones de pago (Facebook Ads) para promocionar la publicación y llegar a más personas.</td>
  </tr>
  <tr>
    <td><b>Canales de distribución (Web y/o Móvil)</b></td>
    <td>Plataforma Web (Responsive) y futura App Móvil.</td>
    <td>Plataforma Web clásica.</td>
    <td>Plataforma Web y aplicación móvil altamente desarrollada (iOS/Android).</td>
    <td>Plataforma Web y App Móvil de Facebook.</td>
  </tr>

  <tr>
    <td rowspan="4"><b>Análisis SWOT</b></td>
    <td><b>Fortalezas</b></td>
    <td>Especialización en portafolios sin la complejidad de TikTok/Instagram. Facilidad de uso para no nativos digitales. Contacto directo por WhatsApp que acelera las ventas.</td>
    <td>Alcance a nivel nacional, nombre de dominio muy fácil de recordar y costo de entrada nulo.</td>
    <td>Marca líder indiscutible en su nicho. Base de datos enorme de clientes dispuestos a gastar. Herramientas complementarias muy completas.</td>
    <td>Audiencia cautiva de millones de usuarios diarios. Familiaridad total con la interfaz. Cero barreras de entrada.</td>
  </tr>
  <tr>
    <td><b>Debilidades</b></td>
    <td>Startup nueva que debe lidiar con el "problema del huevo y la gallina" (necesita profesionales para atraer clientes y viceversa). Depende de la adopción tecnológica inicial.</td>
    <td>Diseño web desactualizado, bajo tráfico en comparación con redes sociales, falta de herramientas visuales como galerías estructuradas.</td>
    <td>Exclusividad extrema (solo bodas), dejando fuera el rentable mercado de 15 años, cumpleaños y oficios del hogar. Costos prohibitivos para pequeños emprendedores.</td>
    <td>Desorden total. Cero filtros de seguridad o validación profesional, lo que propicia estafas. El algoritmo obliga a republicar constantemente para no desaparecer del feed.</td>
  </tr>
  <tr>
    <td><b>Oportunidades</b></td>
    <td>Digitalizar un sector mayormente informal en Latinoamérica. Posibilidad de expandir rápidamente de eventos a oficios técnicos del hogar una vez validado el modelo.</td>
    <td>Si modernizan su interfaz y añaden sistemas de validación o fotografías, podrían captar a la audiencia que huye de la informalidad de Facebook.</td>
    <td>Tienen el capital para abrir plataformas paralelas dedicadas a otros tipos de eventos, acaparando el mercado general.</td>
    <td>Facebook podría lanzar un "Marketplace Services" con perfiles verificados y reseñas, imitando el modelo de directorios formales.</td>
  </tr>
  <tr>
    <td><b>Amenazas</b></td>
    <td>Resistencia al cambio por parte de profesionales que prefieren seguir usando Facebook por costumbre, a pesar de sus fallas. Falta de financiamiento inicial para marketing masivo.</td>
    <td>El crecimiento de plataformas más modernas y visuales (como Servify) que dejen obsoleta su estructura de "clasificados de texto".</td>
    <td>Crisis económicas que reduzcan drásticamente el presupuesto para bodas de lujo, afectando el pago de suscripciones de sus proveedores.</td>
    <td>Pérdida de credibilidad por aumento de estafas en su plataforma, llevando a los usuarios a buscar directorios especializados y seguros.</td>
  </tr>
</table>

## 2.1.2. Estrategias y tácticas frente a competidores

Servify cuenta con una ventaja clara frente a sus competidores: encuentra el punto de equilibrio exacto entre la profesionalidad de un directorio premium y la accesibilidad de una red social. Frente a Matrimonio.com.pe, que cobra planes costosos y se limita exclusivamente al sector de bodas, Servify elimina esa barrera económica con su modelo freemium y abarca todo el espectro de eventos privados y oficios locales, capturando a un mercado masivo de emprendedores que actualmente se encuentra desatendido.

Frente a Facebook Marketplace, que domina por su inmenso tráfico pero sufre de alta informalidad y desorden, la táctica es posicionar a Servify como la alternativa "segura y estructurada". La estrategia no es intentar robarle el tráfico diario a Facebook, sino ofrecer a los profesionales una herramienta (su enlace de perfil de Servify) que puedan compartir en sus propias redes sociales o WhatsApp. De esta manera, se garantiza a los clientes finales un ecosistema limpio, con galerías ordenadas y reseñas verificadas que eliminen el miedo a las estafas.

Respecto a Recomiendame.pe, que es una opción local pero estática y basada solo en texto, la estrategia es diferenciarse radicalmente mediante el diseño visual y la experiencia de usuario (UX). Servify priorizará las galerías de imágenes de alta calidad y la integración directa con WhatsApp para cotizaciones inmediatas, demostrando ser una herramienta diseñada específicamente para cerrar ventas de forma ágil.

La táctica central de Servify debe basarse en el crecimiento orgánico impulsado por la propia comunidad. Al ofrecer un portafolio digital gratuito y fácil de usar, los propios trabajadores independientes actuarán como embajadores de la marca al compartir sus perfiles con prospectos, generando un efecto de red (network effect) que construya credibilidad y atraiga tanto a más profesionales como a clientes finales.

## 2.2. Entrevistas

Con el objetivo de conocer cómo los profesionales independientes gestionan actualmente la captación de clientes y qué dificultades enfrentan los usuarios al buscar servicios, se llevaron a cabo entrevistas dirigidas a nuestros dos segmentos principales: trabajadores independientes (proveedores de eventos y oficios) y clientes finales (organizadores de eventos y dueños de hogar). Para cada segmento se diseñaron preguntas abiertas que permitieran entender sus hábitos, su nivel de dominio tecnológico, cómo manejan la desconfianza en contrataciones por internet y su disposición a utilizar un directorio centralizado.

La información recopilada fue revisada y organizada para identificar comportamientos recurrentes, problemas comunes y necesidades no cubiertas. Este análisis permitió obtener una visión más clara sobre cómo los profesionales luchan y se frustran contra los algoritmos de las redes sociales, y cómo los clientes finales pierden tiempo valioso ante la falta de catálogos formales y validados.

A partir de estos hallazgos, se pudieron establecer criterios clave para el desarrollo de Servify, asegurando que la solución responda a situaciones reales, elimine la fricción en el proceso de búsqueda y aporte un valor contundente: mayores ingresos y formalidad para el profesional, y seguridad y rapidez para el cliente.

### 2.2.1. Diseño de entrevistas

En esta sección se define la información a recolectar de los segmentos objetivo. Los datos básicos de los entrevistados serán registrados mediante un formulario, el cual estará disponible a través del siguiente enlace: [INSERTA_TU_LINK_DE_GOOGLE_FORMS_AQUI]

**Entrevistas Segmento 1: Trabajadores independientes y de oficios**
1. ¿Cuál es su nombre y apellido?
2. ¿Cuál es su edad?
3. ¿Qué sistema operativo usa en su dispositivo móvil (ej. Android, iOS)?
4. ¿Qué sistema operativo usa en su computadora y/o laptop (ej. Windows, macOS)?
5. ¿Podría contarnos a qué oficio se dedica y cuánto tiempo lleva ofreciendo sus servicios?
6. ¿Cómo consigue la mayoría de sus clientes actualmente (boca a boca, referidos, redes sociales)?
7. ¿Qué herramientas utiliza para mostrar su trabajo o portafolio a los clientes potenciales?
8. ¿Qué tan difícil le resulta captar nuevos clientes a través de redes sociales como Facebook o Instagram?
9. ¿Cuáles son las mayores frustraciones que enfrenta al intentar promocionar su negocio en internet?
10. ¿Alguna vez ha perdido un contrato por no tener un catálogo o portafolio organizado para mostrar rápidamente?
11. ¿Ha utilizado alguna plataforma o directorio web para ofrecer sus servicios? ¿Cuál fue su experiencia?
12. Si existiera una plataforma sencilla y exclusiva para crear su portafolio sin necesidad de saber usar redes sociales, ¿cree que le ayudaría?
13. ¿Qué tan importante es para usted que los clientes puedan contactarlo directamente a su WhatsApp con un solo clic?
14. ¿Le resultaría útil un sistema donde sus clientes anteriores puedan dejarle reseñas y calificaciones de 1 a 5 estrellas?
15. ¿Qué información considera indispensable que debe ir en su perfil profesional digital?
16. ¿Qué lo desmotivaría o qué preocupaciones tendría al registrarse en una nueva plataforma de oficios?
17. ¿Estaría dispuesto a pagar una suscripción económica para destacar su perfil y aparecer en los primeros resultados de búsqueda? ¿Por qué?

**Entrevistas Segmento 2: Clientes finales (Organizadores y hogares)**
1. ¿Cuál es su nombre y apellido?
2. ¿Cuál es su edad?
3. ¿Qué sistema operativo usa en su dispositivo móvil (ej. Android, iOS)?
4. ¿Qué sistema operativo usa en su computadora y/o laptop (ej. Windows, macOS)?
5. ¿Podría contarnos un poco sobre usted y con qué frecuencia suele organizar eventos o requerir servicios de oficios para el hogar?
6. Cuando necesita contratar a un profesional independiente (ej. un gasfitero, un DJ, un decorador), ¿cómo suele buscarlo?
7. ¿Qué tan importante es para usted ver fotos claras o el portafolio del trabajador antes de decidir contratarlo?
8. ¿Alguna vez ha tenido una mala experiencia, mal servicio o ha sido estafado al contratar a alguien por internet o redes sociales? ¿Qué pasó?
9. ¿Cuáles son las mayores frustraciones que tiene al buscar talento local en plataformas desorganizadas como Facebook Marketplace?
10. ¿Qué factores le generan mayor confianza al momento de decidir a qué profesional contactar?
11. Si existiera un directorio web exclusivo de profesionales verificados con fotos de sus trabajos, ¿cómo lo utilizaría?
12. ¿Qué tanto valora poder leer reseñas reales de otras personas antes de contactar a un trabajador independiente?
13. ¿Le parece más cómodo contactar al proveedor a través de un chat interno de la página o prefiere que la web lo redirija a su WhatsApp?
14. ¿Qué tipo de filtros le gustaría tener al buscar un servicio (precio, ubicación, calificación por estrellas)?
15. ¿Qué características debería tener esta plataforma para que usted la prefiera por encima de seguir buscando en grupos de Facebook?
16. ¿Qué aspecto le haría desconfiar de una plataforma de este tipo?
17. ¿Estaría dispuesto a recomendar esta plataforma a sus conocidos si le ayuda a encontrar un buen profesional de forma rápida y segura?