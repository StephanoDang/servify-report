<div align="center">

  <img src="https://via.placeholder.com/150?text=Servify+Logo" alt="Logo Servify" width="120">

  <p><strong>Proyecto Personal de Portafolio</strong><br>
  Desarrollo de Aplicaciones Web y Arquitectura de Software</p>

  <br>

<h3><strong>Informe Técnico de Producto: Servify</strong></h3>
<h4>Marketplace Web basado en Arquitectura de Microservicios para resolver la informalidad y la fricción en la contratación de servicios en el sector de eventos privados en Lima Metropolitana.</h4>

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
| 1.0 | 30/07/2026 | Stephano Dang | Creación inicial del documento. Definición del Startup Profile. |
| 1.1 | 25/08/2026 | Stephano Dang | Reestructuración al sector exclusivo de eventos y 3 segmentos objetivo. |
| 1.2 | 26/08/2026 | Stephano Dang | Integración del modelo transaccional (contratos digitales y cobro de comisión). |

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

**Servify** es un Marketplace Web transaccional diseñado para resolver la informalidad y la fricción en la contratación de servicios dentro del sector de eventos privados en Lima Metropolitana. A través de su plataforma intuitiva, la aplicación centraliza la oferta y demanda, transformando los tratos informales e inseguros (realizados tradicionalmente por WhatsApp) en un ecosistema digital donde las reservas se formalizan mediante **contratos digitales integrados**.

La plataforma está diseñada para atender a un ecosistema de tres perfiles fundamentales:
1. **Cliente:** Quien contrata para su evento.
2. **Proveedor del servicio de eventos (Organizador):** El profesional que brinda el servicio para el evento y necesita exhibir su portafolio.
3. **Personas que quieran trabajar para el proveedor (Personal de apoyo):** Talento que busca conectar con organizadores de manera segura para trabajar en sus eventos.

**Modelo de Negocio:** Inspirado en plataformas transaccionales exitosas (como Airbnb o Booking), Servify actúa como un intermediario seguro. Los clientes y proveedores generan un acuerdo formal dentro de la página web. La plataforma procesa el pago y cobra un pequeño porcentaje de comisión por el servicio de intermediación, garantizando a ambas partes un respaldo legal e institucional ante cancelaciones o incumplimientos.

**Misión:** Impulsar el crecimiento económico y la formalización en la industria de eventos mediante un marketplace seguro que conecte a clientes, proveedores y personal de apoyo, brindando contratos digitales que protejan el dinero y el tiempo de los usuarios.

**Visión:** Ser la plataforma transaccional de eventos de referencia en el Perú, liderando la creación de un ecosistema donde el talento y las necesidades de celebración converjan bajo un marco de confianza, garantías y alta calidad.

### 1.1.2. Perfiles de integrantes del equipo

Al ser un proyecto de portafolio personal, el desarrollo y arquitectura de la plataforma están a cargo de un único creador que asume todos los roles del ciclo de vida del software.

| Perfil | Datos del Desarrollador | Conocimientos y Habilidades |
| :---: | :--- | :--- |
| <img src="images/stephano.jpeg" width="120" style="border-radius: 8px;"><br>**Full-Stack Developer** | **Nombres y Apellidos:**<br>Angelo Stephano Moscoso Bejar | **Stack Tecnológico:**<br>C++, CSS, HTML, Vue.js, SQL, JS.<br><br>**Aportes al Proyecto:**<br>Encargado del diseño de la arquitectura de datos, desarrollo frontend/backend, maquetación de interfaces responsivas y la implementación de la lógica de negocio (incluyendo la pasarela de pagos y generación de contratos). |

## 1.2. Solution Profile

### 1.2.1. Antecedentes y problemática

### Antecedentes
<div style="text-align: justify">

En la industria de eventos privados de Lima Metropolitana, la presencia digital y la formalidad en las contrataciones son factores indispensables que actualmente se encuentran desatendidos. Gran parte de este ecosistema opera en una informalidad crítica. A pesar de que la organización de cumpleaños, quinceañeros, bodas y eventos corporativos mueve grandes sumas de dinero, la falta de una plataforma transaccional y centralizada limita el crecimiento de los proveedores y expone a los clientes a riesgos financieros considerables.

Actualmente, los acuerdos entre clientes y proveedores de eventos se limitan a "quedar" de palabra mediante mensajes de WhatsApp. Al no existir un contrato formal que respalde a ninguna de las partes, los clientes se exponen a estafas (pagos por adelantado donde el proveedor no asiste o brinda un servicio deficiente), y los proveedores se arriesgan a cancelaciones de última hora sin recibir la remuneración justa por reservar la fecha.

Por otro lado, cuando un proveedor o agencia necesita reclutar personas que quieran trabajar para su evento (personal de apoyo como DJs, animadoras o mozos), se ven obligados a recurrir a grupos informales de Facebook. Esta dinámica carece de garantías legales y filtros de confianza, exponiendo al organizador al ausentismo y al trabajador independiente a cancelaciones e intermediarios abusivos. Esta desorganización logística genera una alta fricción y dificultad en la contratación de servicios, evidenciando la necesidad urgente de una plataforma web que no solo sirva como directorio o vitrina visual, sino que asegure la transacción completa mediante contratos digitales vinculantes.

</div>

### Problemática

<div style="text-align: justify">
Para entender a profundidad la necesidad que impulsa este proyecto y justificar el desarrollo del modelo transaccional, se aplicó la técnica de análisis de las 5W's + 2H's:

### 5W's
**What (¿Cuál es el problema?):**
La industria de eventos locales sufre de alta fricción operativa y riesgo financiero en la contratación. Los acuerdos informales por WhatsApp carecen de validez, generando estafas, desconfianza y cancelaciones de última hora.

**When (¿Cuándo ocurre el problema?):**
Al momento de cerrar un trato y realizar el pago del anticipo para asegurar un servicio (especialmente en temporadas altas de fiestas y eventos).

**Where (¿Dónde ocurre el problema?):**
En el sector de servicios y eventos privados en el mercado local de Lima Metropolitana.

**Who (¿A quién o quiénes afecta el problema?):**
* **Clientes:** Familias y empresas que arriesgan su dinero al no tener contratos que garanticen el servicio.
* **Proveedores de eventos:** Organizadores que pierden ingresos por cancelaciones informales.
* **Personas que quieran trabajar:** Talento independiente excluido de contrataciones seguras.

**Why (¿Por qué sucede el problema?):**
Porque no existe una pasarela transaccional especializada en eventos que brinde contratos digitales vinculantes para proteger el dinero del cliente y el tiempo del proveedor, dejando las negociaciones relegadas a redes sociales no reguladas.

### 2H's
**How (¿Cómo aparece el problema?):**
Aparece como desconfianza mutua. El cliente teme depositar a un desconocido, y el proveedor teme reservar una fecha sin garantías reales.

**How Much (¿Cuánto afecta el problema?):**
Impacta directamente en el riesgo financiero para el cliente y en la pérdida significativa de ingresos para los proveedores ante incumplimientos sin penalidad formal.
</div>

### 1.2.2. Lean UX Process

#### 1.2.2.1. Lean UX Problem Statements

**Problema 1: La informalidad transaccional entre Clientes y Proveedores**
El estado actual de la contratación de servicios para eventos privados en Lima Metropolitana depende casi en su totalidad de acuerdos informales o "de palabra" realizados a través de WhatsApp. Lo que los clientes finales necesitan es una garantía real de que su dinero no será robado y de que el proveedor cumplirá con el servicio el día de su celebración. Por el lado de los proveedores, ellos necesitan asegurar sus ingresos y protegerse legalmente ante clientes que cancelan a última hora sin asumir ninguna penalidad. Hemos observado que la falta de una pasarela formal genera una alta fricción en la contratación de servicios, un clima de desconfianza mutua y un riesgo financiero crítico para ambas partes.

**¿Cómo podríamos diseñar un marketplace transaccional que permita a los clientes y proveedores cerrar sus acuerdos mediante contratos digitales automáticos y pagos seguros, eliminando el riesgo de estafas y garantizando el cumplimiento del evento?**

---

**Problema 2: La desorganización en el reclutamiento del Personal de Apoyo**
El estado actual de la búsqueda y subcontratación de personal de apoyo (animadoras, DJs, bartenders, mozos) obliga a los proveedores de eventos a recurrir a grupos informales de Facebook Marketplace. Lo que los organizadores necesitan es una forma rápida, confiable y verificada de armar su equipo de trabajo (logística) para fechas específicas. A su vez, las personas que quieren trabajar para el proveedor necesitan una vitrina formal para exhibir su talento y conseguir trabajos recurrentes sin depender de intermediarios abusivos. Hemos observado que esta desconexión genera incumplimientos laborales, estrés de última hora para el organizador y estancamiento económico para el trabajador independiente.

**¿Cómo podríamos integrar un módulo de bolsa de trabajo (B2B) dentro del marketplace donde los proveedores puedan reclutar de forma confiable a su equipo, y donde el personal de apoyo pueda construir un portafolio validado por reseñas para postular a estas ofertas?**

#### 1.2.2.2. Lean UX Assumptions

**Assumptions Worksheet**

- **¿Quién es el usuario?**
  Tenemos tres tipos de usuarios principales interconectados: Los **clientes** (personas o empresas que necesitan contratar un servicio para su evento), los **proveedores de servicios de eventos** (organizadores, agencias o profesionales que ejecutan el evento) y las **personas que quieran trabajar para el proveedor** (personal de apoyo como mozos, DJs, animadoras o bartenders).

- **¿Dónde encaja nuestro producto en su trabajo o vida?**
  Para el cliente final, Servify será la herramienta segura "on-demand" a la que acudirán para cotizar, firmar un contrato y reservar su evento sin miedo a estafas. Para el proveedor, será su principal vitrina comercial, gestor de cobros y su bolsa de reclutamiento B2B. Para el personal de apoyo, funcionará como su bolsa de trabajo validada para conseguir "gigs" recurrentes los fines de semana.

- **¿Qué problemas resuelve nuestro producto?**
  El producto resuelve la fricción en la contratación de servicios, la vulnerabilidad financiera (estafas y cancelaciones sin penalidad) generada por "quedar" de manera informal por WhatsApp, y la dificultad logística de los organizadores para reclutar talento de apoyo confiable a última hora.

- **¿Cuándo y cómo es usado nuestro producto?**
  Se utiliza en las etapas de planificación y cierre del evento. El cliente lo usará para realizar búsquedas, firmar el contrato digital y depositar el pago en garantía. El proveedor lo usará para gestionar estas reservas, recibir su dinero tras el evento y publicar ofertas para contratar a su personal. El personal de apoyo lo usará para postular a estas ofertas y armar su portafolio.

- **¿Qué características son importantes?**
  Para generar confianza absoluta, las características clave son: pasarela de pagos integrada, generación automática de contratos digitales vinculantes, creación de perfiles con galerías visuales de carga rápida, un módulo de bolsa de trabajo interno (B2B) y un sistema cruzado de reseñas de 1 a 5 estrellas.

- **¿Cómo debe verse nuestro producto y cómo comportarse?**
  Nuestro producto debe transmitir profesionalismo, seguridad transaccional y confianza (similar a la experiencia de reservar en Airbnb o Booking). Su interfaz debe ser extremadamente limpia e intuitiva, asegurando que ningún usuario sufra fricción tecnológica al momento de vincular su método de pago o firmar un acuerdo.

**Business Assumptions:**

- Creemos que los clientes y los proveedores están dispuestos a cerrar sus acuerdos a través de la plataforma y pagar un pequeño porcentaje de comisión transaccional, siempre y cuando la plataforma les garantice un contrato formal, protección de su dinero y seguridad frente a incumplimientos.
- Creemos que ofrecer contratos digitales automatizados será el principal diferenciador competitivo frente a la informalidad total que predomina en los grupos de Facebook Marketplace en Lima Metropolitana.
- Creemos que al ofrecer portafolios gratuitos a las personas que quieran trabajar para los proveedores (personal de apoyo), estos actuarán como embajadores orgánicos al compartir sus enlaces, atrayendo a los organizadores hacia nuestro ecosistema.
- Nuestro mayor riesgo logístico es mantener el equilibrio simultáneo en los tres lados del marketplace: asegurar que haya suficientes eventos disponibles para el personal de apoyo, suficientes organizadores verificados para los clientes, y suficiente demanda de clientes para mantener a los organizadores pagando la comisión.
- Creemos que las alianzas estratégicas iniciales con gremios locales de eventos o asociaciones de catering en Lima Metropolitana pueden acelerar la adopción de la plataforma por parte de los proveedores.


#### 1.2.2.3. Lean UX Hypothesis Statements

- Creemos que si ofrecemos a los clientes y proveedores de eventos una pasarela de pagos segura con generación automática de contratos digitales, entonces abandonarán la costumbre de "quedar" informalmente por WhatsApp y reducirán drásticamente su riesgo a sufrir estafas o cancelaciones. Sabremos que estamos en lo correcto cuando logremos que al menos el 30% de los usuarios activos cierre su reserva directamente en la plataforma (pagando el porcentaje de comisión) durante los primeros tres meses de lanzamiento.

- Creemos que si integramos un módulo de bolsa de trabajo interna (B2B) exclusivo para los proveedores de servicios de eventos, entonces estos podrán gestionar su logística y reclutar personal de apoyo de manera mucho más rápida y confiable que publicando en grupos de Facebook. Sabremos que estamos en lo correcto cuando las analíticas muestren que el 40% de los proveedores activos utilice el sistema para contratar al menos a un talento verificado por mes.

- Creemos que si proporcionamos a las personas que quieran trabajar para el proveedor (mozos, animadoras, DJs, etc.) la opción de crear un portafolio visual completamente gratuito dentro de un entorno validado, entonces adoptarán la plataforma para escapar de la informalidad y de los intermediarios abusivos. Sabremos que estamos en lo correcto cuando logremos que el 60% del personal de apoyo registrado complete al 100% su galería de fotos, videos y referencias durante su primera semana de uso.

#### 1.2.2.4. Lean UX Canvas

<div align="center">
  <img src="images/lean_ux.png" alt="Lean UX Canvas de Servify">
</div>

## 1.3. Segmentos Objetivo

| | Segmento 1: Cliente | Segmento 2: Proveedor del Servicio de Eventos | Segmento 3: Personas que quieran trabajar para el proveedor |
| :--- | :--- | :--- | :--- |
| **Variables** | Personas naturales, familias o representantes de empresas que requieren contratar y organizar proveedores verificados para eventos privados (cumpleaños, quinceañeros, reuniones corporativas). | Profesionales independientes, emprendedores o agencias que brindan servicios integrales para la planificación, decoración y ejecución de eventos en general. | Trabajadores independientes y talento técnico (animadoras, catering, bartenders, DJs, mozos) que buscan conectarse con organizadores para trabajar por horas o evento. |
| **Geográfica** | Ubicados principalmente en zonas urbanas y suburbanas de Lima Metropolitana, en distritos con alta actividad social, residencial y empresarial. | Ubicados en Lima Metropolitana. Con capacidad logística para trasladarse y cubrir eventos en distintos distritos de la capital. | Residentes de Lima Metropolitana. Con disponibilidad para desplazarse a los locales o viviendas donde se realice la celebración de manera puntual. |
| **Demográfica** | **Edad:** 25-55 años. **Género:** Mixto. **Educación:** Secundaria completa o superior. **Ingresos:** Medio a alto. **Estado civil:** Padres de familia, parejas, asistentes administrativos. | **Edad:** 25-50 años. **Género:** Mixto. **Educación:** Empírica, técnica o superior. **Ingresos:** Variables. **Ocupación:** Emprendedores y dueños de pequeñas empresas de eventos. | **Edad:** 18-45 años. **Género:** Mixto. **Educación:** Básica, empírica o técnica. **Ingresos:** Variables (pago por evento). **Perfil:** Estudiantes, artistas o técnicos. |
| **Psicológica** | Tienen temor a las estafas online y a los pagos por adelantado sin respaldo legal. Valoran la confianza, la puntualidad y la seguridad de tener un contrato formal. Prefieren tomar decisiones basadas en reseñas verificadas y catálogos visuales. | Buscan formalizar sus ventas, asegurar ingresos constantes y escalar sus negocios. Sienten frustración ante las cancelaciones de última hora por tratos informales. Valoran herramientas que les ahorren tiempo y brinden protección legal. | Buscan estabilidad en el flujo de trabajo continuo y reconocimiento. Sienten frustración al ser estafados, no recibir sus pagos o lidiar con intermediarios abusivos. Desean pertenecer a un entorno seguro y validado. |
| **Función de comportamiento** | Uso frecuente de internet y comercio electrónico. Están dispuestos a pagar una pequeña comisión si la plataforma asegura su dinero y garantiza el cumplimiento del evento. Su objetivo es encontrar proveedores reduciendo la fricción y el estrés. | Adoptarán la plataforma tecnológica para gestionar sus ventas con contratos y evitar clientes irresponsables. Buscan agilizar sus procesos operativos y reclutar personal de apoyo de manera confiable cuando la demanda lo requiere. | Alto uso de redes sociales (Instagram, TikTok) para intentar captar trabajos, pero con baja conversión. Utilizarán la plataforma para mantener un portafolio activo y postular a ofertas directas de los proveedores. |

---

<div style="page-break-after: always;"></div>

# Capítulo II: Requirements Elicitation & Analysis

## 2.1. Competidores

### 1. Directorios de Anuncios Locales y Clasificados Digitales
<div style="text-align: justify">
Existen múltiples directorios web a nivel nacional enfocados en la búsqueda y recomendación de servicios generales. Estas plataformas permiten a los usuarios buscar requerimientos específicos y a los trabajadores publicar anuncios básicos basados en texto sobre lo que hacen. 

En cuanto a costos y modelo de negocio, son alternativas gratuitas o de muy bajo costo; sin embargo, no cuentan con un alto nivel de popularidad ni adopción masiva en el rubro específico de eventos. Al ser estáticos, carecen del impacto visual (galerías dinámicas), las pasarelas de pago y la generación de contratos digitales que son vitales para garantizar seguridad en un evento privado. Esta carencia tecnológica limita drásticamente la exposición y el retorno real que obtienen los organizadores y el personal de apoyo al registrarse allí.
</div>

### 2. Matrimonio.com.pe
<div style="text-align: justify">
Es una de las plataformas web y móviles más grandes en el rubro de eventos sociales en Latinoamérica. Funciona como un directorio súper especializado donde los proveedores de servicios pueden crear un perfil profesional, subir galerías de fotos de alta calidad, utilizar herramientas de cotización y recibir reseñas detalladas de sus clientes. 

Su modelo de negocio es freemium. Aunque crear un perfil básico es gratuito, la plataforma está altamente saturada, obligando a los profesionales a pagar planes premium costosos para aparecer en los primeros resultados. Además, su principal limitante es que está exclusivamente enfocada en bodas, dejando totalmente por fuera el gigantesco y rentable mercado de cumpleaños, quinceañeros y eventos corporativos en Lima Metropolitana. Asimismo, su enfoque es solo de directorio (vitrina), careciendo de un modelo transaccional que asegure el dinero del cliente y de un espacio para que el personal de apoyo postule a trabajos.
</div>

### 3. Facebook Marketplace y Grupos de Facebook
<div style="text-align: justify">
Aunque no es una plataforma especializada en la gestión de eventos, Facebook (a través de sus Grupos locales y Marketplace) es actualmente el principal ecosistema por defecto al que recurren tanto los organizadores como el personal de apoyo para intentar captar contratos. Permite subir fotos y colocar descripciones rápidas del servicio ofrecido. 

Si bien es una herramienta totalmente gratuita y de tráfico masivo, carece de una estructura profesional para portafolios y transacciones. Los profesionales se enfrentan a la barrera de los algoritmos de redes sociales, la necesidad constante de "republicar" para no desaparecer y la altísima informalidad. Al no existir pasarelas de pago seguras ni contratos digitales integrados, los tratos se ven obligados a cerrarse "en el aire" mediante WhatsApp, lo que provoca una alta fricción en la contratación de servicios, dejando a los tres segmentos vulnerables a estafas e incumplimientos sin ninguna garantía de protección.
</div>

### 2.1.1. Análisis Competitivo

<table>
  <tr>
    <th colspan="6">Competitive Analysis Landscape</th>
  </tr>
  <tr>
    <td colspan="2"><b>¿Por qué llevar a cabo este análisis?</b></td>
    <td colspan="4">El objetivo de este análisis es entender cómo interactúan los tres segmentos (clientes, proveedores de eventos y personal de apoyo) en el mercado actual. Identificar las fallas críticas de las plataformas existentes (altos costos, informalidad absoluta, ausencia de garantías legales) es vital para justificar el desarrollo de Servify como un marketplace transaccional que resuelva definitivamente la fricción en la contratación de servicios en Lima Metropolitana.</td>
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
    <td><b>Servify</b><br>Lima Metropolitana, Perú</td>
    <td>
      <b>Matrimonio.com.pe</b>
      <br>Latinoamérica
    </td>
    <td>
      <b>Facebook Marketplace y Grupos</b>
      <br>Global
    </td>
    <td>
      <b>Directorios y Clasificados Web</b>
      <br>Perú
    </td>
  </tr>

  <!-- PERFIL -->
  <tr>
    <td rowspan="2"><b>Perfil</b></td>
    <td><b>Overview</b></td>
    <td>Marketplace Web basado en Arquitectura de Microservicios diseñado para resolver la informalidad y la fricción en la contratación de servicios. Conecta a clientes con proveedores, y a proveedores con personal de apoyo mediante contratos digitales automáticos.</td>
    <td>Directorio web y móvil altamente especializado en el rubro de bodas. Funciona como vitrina donde los proveedores crean perfiles premium con galerías de alta calidad, pero no procesan el pago transaccional completo del servicio.</td>
    <td>Sección de compra/venta y grupos comunitarios dentro de la red social. Usada masivamente por proveedores y personal de apoyo para publicar fotos rápidas. Todo trato es externo e informal (vía WhatsApp).</td>
    <td>Directorios web a nivel nacional enfocados en publicar anuncios textuales sobre servicios. Funcionan como una guía telefónica digital o sección de clasificados modernos sin validación.</td>
  </tr>
  <tr>
    <td><b>Ventaja competitiva<br>¿Qué valor ofrece a los clientes?</b></td>
    <td>Seguridad absoluta. Soluciona la fricción operativa mediante contratos digitales y pagos seguros (modelo Booking/Airbnb). El trato no queda "en el aire", protegiendo el dinero del cliente y el tiempo del proveedor.</td>
    <td>Prestigio, confianza y herramientas adicionales de planificación. Si un proveedor está posicionado aquí, garantiza un flujo de clientes listos para invertir fuerte.</td>
    <td>Tráfico inmenso y cero barreras de entrada. El usuario no necesita descargar nada nuevo porque ya utiliza la red social todos los días.</td>
    <td>Gratuidad total y mucha facilidad técnica para dejar un número de contacto publicado.</td>
  </tr>

  <!-- PERFIL DE MARKETING -->
  <tr>
    <td rowspan="2"><b>Perfil de Marketing</b></td>
    <td><b>Mercado objetivo</b></td>
    <td>Clientes (celebraciones privadas), Proveedores del servicio de eventos (organizadores), y Personas que quieran trabajar para el proveedor (mozos, animadoras, DJs) en Lima Metropolitana.</td>
    <td>Exclusivamente parejas comprometidas dispuestas a invertir fuertemente en su boda, y proveedores con presupuestos de marketing moderados/altos.</td>
    <td>Público general. Cualquier persona con internet que busque soluciones rápidas y talento independiente que busque "recursearse" en su localidad.</td>
    <td>Usuarios tradicionales que buscan resolver requerimientos esporádicos a muy bajo costo o técnicos sin conocimientos de redes sociales.</td>
  </tr>
  <tr>
    <td><b>Estrategias de marketing</b></td>
    <td>Efecto de red impulsado por la seguridad: Atraer al personal de apoyo ofreciendo un perfil gratis para captar proveedores, y atraer a los clientes ofreciéndoles protección antifraude sobre su dinero.</td>
    <td>Fuerte inversión en SEO/SEM, organización de ferias presenciales de novios, publicidad tradicional y branding aspiracional muy potente.</td>
    <td>El marketing lo hace el ecosistema de la app. Facebook retiene a la audiencia mediante grupos y notificaciones cruzadas.</td>
    <td>Posicionamiento SEO local (búsquedas en Google tipo "animadora barata en Lima") y listados orgánicos.</td>
  </tr>

  <!-- PERFIL DE PRODUCTO -->
  <tr>
    <td rowspan="3"><b>Perfil de Producto</b></td>
    <td><b>Productos & Servicios</b></td>
    <td>Perfiles visuales, bolsa interna de trabajo (B2B), pasarela de pagos integrada, contratos automáticos descargables, y sistema de reseñas de doble vía.</td>
    <td>Perfiles premium, cotizador interno, agenda de citas, foros de comunidad y sellos de calidad (premios anuales).</td>
    <td>Publicaciones efímeras en un feed estilo clasificados, interacción en grupos locales de eventos e integración directa con Messenger.</td>
    <td>Fichas de contacto muy básicas con título, descripción del servicio y zona de cobertura. Carecen de galerías visuales estructuradas.</td>
  </tr>
  <tr>
    <td><b>Precios & Costos</b></td>
    <td>Modelo Transaccional. Inscripción gratuita. Se cobra un pequeño porcentaje de comisión únicamente si el contrato/reserva se cierra con éxito a través de la plataforma.</td>
    <td>Modelo Freemium costoso. Aparecer en los resultados requiere pagar suscripciones mensuales o anuales elevadas para destacar.</td>
    <td>100% gratuito para publicar. Opciones de pago (Ads) para promocionar la publicación temporalmente.</td>
    <td>Gratuito o con opciones de pago (micropagos) para mantener el anuncio en la cima del directorio.</td>
  </tr>
  <tr>
    <td><b>Canales de distribución</b></td>
    <td>Plataforma Web (Responsive).</td>
    <td>Plataforma Web y App Móvil (iOS/Android).</td>
    <td>Plataforma Web y App Móvil.</td>
    <td>Plataforma Web clásica.</td>
  </tr>

  <!-- ANÁLISIS SWOT -->
  <tr>
    <td rowspan="4"><b>Análisis SWOT</b></td>
    <td><b>Fortalezas</b></td>
    <td>Integra contratos vinculantes y pagos, eliminando el miedo a las estafas. Abarca todo tipo de eventos (no solo bodas). Cubre la necesidad B2B al incorporar al personal de apoyo en el mismo ecosistema.</td>
    <td>Marca líder en su nicho. Base de datos enorme de proveedores de alto nivel y clientes con alto presupuesto.</td>
    <td>Audiencia cautiva de millones de usuarios diarios. Familiaridad total con la interfaz. Cero curvas de aprendizaje.</td>
    <td>Nombre de dominio fácil de recordar y costo de entrada totalmente nulo para el publicante.</td>
  </tr>
  <tr>
    <td><b>Debilidades</b></td>
    <td>Reto logístico: equilibrar la oferta y demanda de los 3 segmentos simultáneamente. Necesidad de educar al usuario para que pague dentro del sistema y no decida evadir la comisión yéndose a WhatsApp.</td>
    <td>Exclusividad extrema (ignora cumpleaños, corporativos, 15 años). Costos fijos prohibitivos para pequeños proveedores de eventos.</td>
    <td>Desorden total. Cero filtros de seguridad o validación. Tratos informales que propician un altísimo índice de estafas, robos y cancelaciones.</td>
    <td>Diseño web desactualizado. Incapacidad para mostrar galerías visuales (videos/fotos), lo cual es el factor decisivo para vender un evento.</td>
  </tr>
  <tr>
    <td><b>Oportunidades</b></td>
    <td>Digitalizar y formalizar un mercado multimillonario en Lima Metropolitana que actualmente opera casi al 100% en la sombra de la informalidad.</td>
    <td>Tienen el capital para abrir plataformas paralelas dedicadas a fiestas infantiles o eventos corporativos.</td>
    <td>Facebook podría implementar pasarelas de pago y contratos integrados dentro de sus grupos de Marketplace en un futuro.</td>
    <td>Si modernizan su interfaz y añaden soporte multimedia, podrían captar a la audiencia que huye de Facebook.</td>
  </tr>
  <tr>
    <td><b>Amenazas</b></td>
    <td>Fuerte resistencia al cambio por parte de proveedores que prefieren el riesgo de la informalidad de Facebook con tal de no pagar una pequeña comisión por el contrato.</td>
    <td>Crisis económicas que reduzcan drásticamente la capacidad de inversión de las parejas, afectando el pago de suscripciones.</td>
    <td>Pérdida de credibilidad por el aumento descontrolado de perfiles falsos, forzando a los usuarios a migrar a plataformas cerradas y verificadas (como Servify).</td>
    <td>Ser desplazados y olvidados completamente por el uso de plataformas altamente visuales como Instagram o TikTok.</td>
  </tr>
</table>

## 2.1.2. Estrategias y tácticas frente a competidores

Servify cuenta con una ventaja clara frente a sus competidores al abarcar la cadena logística completa de un evento y resolver el dolor principal del mercado: la inseguridad financiera. Frente a Matrimonio.com.pe, que cobra suscripciones de alto costo y se limita exclusivamente a las bodas, Servify democratiza el acceso abarcando fiestas infantiles, cumpleaños, quinceañeros y eventos corporativos en Lima Metropolitana. Al eliminar la barrera de entrada (suscripción gratuita) y cobrar solo una pequeña comisión por contrato cerrado, atrae a un mercado masivo de emprendedores y agencias que actualmente se encuentran excluidos de las plataformas premium.

Frente a Facebook Marketplace y sus grupos informales (el ecosistema por defecto actualmente), que dominan por su inmenso tráfico pero sufren de alta informalidad, desorden y estafas, la táctica es posicionar a Servify como un entorno "blindado y transaccional". La estrategia no es intentar competir directamente por el tráfico diario de Facebook, sino ofrecer a los proveedores una herramienta transaccional (su enlace de perfil de Servify) que puedan compartir en sus propias redes sociales o WhatsApp. De esta manera, cuando un cliente quiera contratarlos, lo hará a través de la pasarela de pagos de Servify, garantizando un contrato digital vinculante que proteja el dinero del cliente y asegure el pago al proveedor. 

Respecto a los directorios web estáticos y genéricos, la estrategia es diferenciarse radicalmente mediante la integración de una bolsa de trabajo B2B. Servify no solo es una vitrina hacia el cliente final, sino un ecosistema interconectado. 

La táctica central de Servify debe basarse en el crecimiento orgánico (efecto de red) impulsado por la seguridad y la propia comunidad. Al ofrecer un portafolio digital gratuito al **Personal de apoyo** (Segmento 3), estos actuarán como embajadores, atrayendo orgánicamente a los **Proveedores de eventos** (Segmento 2) que buscan reclutar talento seguro. Una vez que los organizadores estén consolidados con portafolios de alta calidad y reseñas, el catálogo será lo suficientemente robusto y confiable para atraer masivamente a los **Clientes finales** (Segmento 1), consolidando así el marketplace para resolver la informalidad y la fricción en la contratación de servicios.

## 2.2. Entrevistas

Con el objetivo de validar las hipótesis, conocer cómo los profesionales gestionan actualmente la captación de clientes y qué fricciones enfrentan al buscar servicios, se llevaron a cabo entrevistas dirigidas a nuestros tres segmentos principales: Clientes, Proveedores del servicio de eventos y Personas que quieran trabajar para el proveedor. 

Para cada segmento se diseñaron baterías de preguntas abiertas detalladas que permitieran entender sus hábitos, su nivel de dominio tecnológico, cómo manejan la desconfianza en contrataciones informales por WhatsApp y su disposición a utilizar un marketplace transaccional. La información recopilada permitirá establecer los criterios clave para el desarrollo del MVP de Servify, asegurando que la solución conecte de manera eficiente la oferta y la demanda, aporte formalidad al talento independiente y garantice seguridad transaccional a todas las partes involucradas.

### 2.2.1. Diseño de entrevistas

En esta sección se define la información a recolectar de los segmentos objetivo. Los datos básicos de los entrevistados serán registrados mediante un formulario, el cual estará disponible a través del siguiente enlace: [INSERTA_TU_LINK_DE_GOOGLE_FORMS_AQUI]

**Entrevistas Segmento 1: Cliente (Quien contrata para su evento)**
1. ¿Cuál es su nombre y apellido?
2. ¿Cuál es su edad?
3. ¿Qué sistema operativo usa en su dispositivo móvil (ej. Android, iOS)?
4. ¿Qué sistema operativo usa en su computadora y/o laptop (ej. Windows, macOS)?
5. ¿Con qué frecuencia organiza o apoya en la organización de eventos privados (cumpleaños, quinceañeros, reuniones corporativas)?
6. Cuando necesita contratar a un proveedor de servicios para una fiesta, ¿cómo suele buscarlo actualmente?
7. ¿Qué tan importante es para usted ver un portafolio ordenado (fotos y videos claros) antes de decidir contratar a alguien?
8. ¿Alguna vez ha tenido una mala experiencia, incumplimiento o ha sido estafado al contratar a alguien "de palabra" por internet o WhatsApp? ¿Qué pasó?
9. ¿Cuáles son las mayores frustraciones que tiene al buscar talento local en plataformas desorganizadas como grupos de Facebook?
10. ¿Qué factores le generan mayor confianza al momento de decidir realizar un pago por adelantado a un proveedor de eventos?
11. ¿Estaría dispuesto a realizar la reserva de su evento a través de nuestra página web, pagando una pequeña comisión, si esto le garantiza un contrato formal y la seguridad de que su dinero está protegido si el proveedor le falla?
12. ¿Qué tanto valora poder leer reseñas reales de otras personas antes de contactar a un organizador?
13. ¿Qué tipo de filtros le gustaría tener al buscar un servicio (precio, ubicación, calificación, tipo de evento)?
14. ¿Qué características debería tener esta plataforma para que usted la prefiera por encima de seguir buscando en Facebook?
15. ¿Qué aspecto le haría desconfiar de realizar un pago a través de un marketplace de eventos?

**Entrevistas Segmento 2: Proveedor del Servicio de Eventos (Organizadores)**
1. ¿Cuál es su nombre y apellido?
2. ¿Cuál es su edad?
3. ¿Qué sistema operativo usa en su dispositivo móvil?
4. ¿Qué sistema operativo usa en su computadora y/o laptop?
5. ¿Qué tipos de eventos suele organizar y cuánto tiempo lleva ofreciendo sus servicios?
6. ¿Cómo consigue la mayoría de sus clientes actualmente y qué herramientas usa para mostrar su portafolio?
7. ¿Qué tan frustrante o difícil le resulta la necesidad de lidiar con algoritmos y crear contenido viral en redes sociales (TikTok/Instagram) para conseguir clientes?
8. ¿Le ha pasado que un cliente le cancela a última hora por haber "quedado" solo por WhatsApp sin un contrato formal de por medio? ¿Cómo le afectó?
9. ¿Estaría de acuerdo en ceder un pequeño porcentaje de comisión a la plataforma si esta le asegura el pago puntual del cliente y emite un contrato digital que lo respalde legalmente?
10. Cuando tiene un evento grande y necesita subcontratar personal de apoyo urgente (bartenders, DJs, animadoras), ¿cómo los encuentra?
11. ¿Ha tenido problemas por falta de compromiso o ausentismo por parte del personal de apoyo contratado de manera informal en grupos de Facebook?
12. Si existiera una plataforma que le permita exhibir su portafolio a clientes y, al mismo tiempo, publicar ofertas para contratar personal de apoyo verificado, ¿le sería útil?
13. ¿Qué información considera indispensable que debe ir en su perfil profesional digital para convencer al cliente?
14. ¿Qué lo desmotivaría o qué preocupaciones tendría al registrarse en un nuevo marketplace transaccional?

**Entrevistas Segmento 3: Personas que quieran trabajar para el proveedor (Personal de apoyo)**
1. ¿Cuál es su nombre y apellido?
2. ¿Cuál es su edad?
3. ¿Qué sistema operativo usa en su dispositivo móvil?
4. ¿Qué sistema operativo usa en su computadora y/o laptop?
5. ¿Cuál es su talento o servicio específico (DJ, animador, catering, bailarín, mozo) y hace cuánto tiempo lo ofrece?
6. ¿Cómo se entera normalmente de oportunidades de trabajo o "gigs" para participar en eventos los fines de semana?
7. ¿Cuenta con un portafolio o catálogo ordenado (videos/fotos) para mostrarle a los organizadores cuando le piden referencias de su trabajo?
8. ¿Qué tan difícil le resulta conseguir que proveedores y organizadores formales conozcan su trabajo sin depender de intermediarios abusivos?
9. ¿Alguna vez le han cancelado a última hora, cambiado las condiciones o no le han pagado tras ser contactado informalmente por redes sociales?
10. ¿Qué le parecería tener un perfil digital gratuito en una plataforma donde los organizadores busquen su talento basándose en su portafolio y reseñas de 1 a 5 estrellas?
11. ¿Estaría dispuesto a mantener su perfil actualizado si sabe que de ahí provendrán sus principales ofertas de trabajo formales?
12. ¿Qué funciones o características le gustaría que tuviera esta plataforma para que realmente la use como su herramienta principal de empleo?
13. ¿Qué le generaría desconfianza al postular a una oferta de trabajo para un evento a través de una página web?
