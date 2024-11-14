## **Pre-preparación**

- En primer lugar, debes comprender a fondo el tipo de puesto al que te postulas. Por ejemplo, debes conocer las responsabilidades y los desafíos que enfrenta un ingeniero de detección si buscas un puesto como tal.
- Asegúrese de conocer bien la empresa a la que se dirige. ¿Va a prestar apoyo a varias empresas al mismo tiempo o la empresa busca un SOC interno?
- Si tienes un amigo que trabaja en la empresa a la que estás postulando, habla con él para averiguar qué tipo de dificultades ha enfrentado en el pasado.
- No compartas tus expectativas salariales durante la entrevista. Una respuesta como: “Creo que mis expectativas salariales están dentro de tus posibilidades. Si todo sale bien, estaré abierto a tus sugerencias en la etapa de propuesta”.
- Asegúrate de conocer el rango salarial del trabajo al que te postulas. Por ejemplo, puedes pedir asesoramiento en Reddit.

‍

## **Preguntas de la entrevista para ingeniero de detección general**

### **¿Cuál es su comprensión del papel de un ingeniero de detección en ciberseguridad?**

Un ingeniero de detección es responsable de diseñar, implementar y mantener sistemas que identifiquen y respondan a las amenazas de seguridad dentro de la red de una organización. Esto implica crear y ajustar reglas de detección, analizar registros de seguridad y desarrollar estrategias para mitigar los riesgos de manera eficaz.

‍

### **¿Puede explicar la diferencia entre los métodos de detección basados ​​en firmas y en anomalías?**

La detección basada en firmas se basa en patrones predefinidos o firmas de amenazas conocidas, mientras que la detección basada en anomalías identifica desviaciones del comportamiento normal. La detección basada en firmas es eficaz contra amenazas conocidas, pero puede pasar por alto ataques nuevos o modificados, mientras que la detección basada en anomalías puede detectar amenazas nuevas, pero puede generar falsos positivos.

‍

### **¿Cómo mantenerse actualizado con las últimas amenazas y técnicas de ataque en el panorama de la ciberseguridad?**

Participo regularmente en foros de ciberseguridad, asisto a conferencias del sector y me suscribo a fuentes de información sobre amenazas. Además, participo activamente en el aprendizaje continuo a través de cursos en línea, seminarios web y lectura de artículos de investigación publicados por expertos en seguridad.

‍

### **Describe un escenario en el que tuviste que desarrollar una regla de detección personalizada para abordar una amenaza de seguridad específica.**

En un puesto anterior, detectamos una serie de intentos de inicio de sesión por fuerza bruta dirigidos contra la puerta de enlace VPN de nuestra organización. Para mitigar esta amenaza, desarrollé una regla de detección personalizada basada en intentos de inicio de sesión fallidos dentro de un período de tiempo específico desde una única dirección IP. Esta regla nos ayudó a identificar y bloquear intentos de inicio de sesión maliciosos de manera más eficaz.

‍

### **¿Cómo abordar el ajuste y la optimización de las reglas de detección para minimizar los falsos positivos y los falsos negativos?**

Comienzo analizando datos históricos y registros de seguridad para comprender el comportamiento típico de nuestra red y de nuestros usuarios. Luego, afino gradualmente las reglas de detección, ajustando los umbrales y los parámetros en función de los patrones observados y los comentarios de los equipos de respuesta a incidentes. El monitoreo regular y los ciclos de retroalimentación son esenciales para garantizar que las reglas de detección sigan siendo efectivas a lo largo del tiempo.

‍

### **¿Qué papel juega la inteligencia sobre amenazas en la ingeniería de detección y cómo aprovecharla de manera eficaz?**

La inteligencia de amenazas proporciona información valiosa sobre amenazas emergentes, técnicas de ataque e indicadores de compromiso (IOC). Como ingeniero de detección, integro fuentes de inteligencia de amenazas en nuestros sistemas de detección para mejorar nuestra capacidad de detectar y responder a amenazas en evolución de manera proactiva. Esto implica correlacionar los IOC con la actividad de la red y ajustar las reglas de detección en consecuencia.

‍

### **¿Cómo abordar el diseño y la implementación de una nueva estrategia de detección para un entorno de red complejo?**

Comienzo realizando una evaluación exhaustiva de la arquitectura de la red, identificando los activos críticos, los posibles vectores de ataque y los controles de seguridad existentes. Con base en este análisis, desarrollo una estrategia de detección integral que incluye una combinación de técnicas de detección basadas en firmas, anomalías y comportamientos adaptadas a las necesidades específicas y al perfil de riesgo de la organización.

‍

**¿Qué papel juega el marco MITRE ATT&CK en la ingeniería de detección?**

El [marco MITRE ATT&CK](https://app.letsdefend.io/training/lessons/mitre-attck-framework) sirve como recurso fundamental en la ingeniería de detección. Proporciona una taxonomía estructurada de tácticas, técnicas y procedimientos (TTP) del adversario que permite a los ingenieros de detección alinear sus estrategias de detección con las amenazas del mundo real.

**¿Cómo contribuye la ingeniería inversa a la ingeniería de detección en ciberseguridad?**

[La ingeniería inversa](https://app.letsdefend.io/training/lessons/reverse-engineering) permite conocer la funcionalidad y el comportamiento de malware y exploits complejos. Al analizar el código malicioso, los ingenieros de detección pueden identificar técnicas de evasión y descubrir funcionalidades ocultas que utilizan los adversarios. 

‍

Si cree que necesita una ruta de aprendizaje para Ingeniería de Detección, puede consultar esta [Capacitación en Ingeniería de Detección](https://app.letsdefend.io/path/detection-engineering-path) :

‍

![](https://cdn.prod.website-files.com/65e1f74aeadd13bc01d31d46/670fd5df63c91df01ee1eb67_670fd56210a92197f70ce349_Screenshot%25202024-10-16%2520at%252011.01.32.png)

‍

## **Preguntas de la entrevista para ingenieros de detección relacionados con Sigma**

### **¿Puedes explicar qué son las reglas Sigma y cómo se utilizan en ciberseguridad?**

Las reglas de Sigma proporcionan un marco genérico y flexible para escribir reglas de detección para eventos de seguridad en diversas fuentes de datos, incluidos registros, tráfico de red y telemetría de puntos finales. Los ingenieros de detección utilizan las reglas de Sigma para estandarizar y simplificar la creación, el uso compartido y la implementación de contenido de detección en diferentes herramientas y plataformas de seguridad.

‍

### **¿Cómo se crean o personalizan las reglas de Sigma para abordar amenazas de seguridad específicas o requisitos organizacionales?**

La creación o personalización de reglas Sigma implica definir condiciones de detección basadas en indicadores de amenazas específicos o comportamientos relevantes para el entorno y los objetivos de seguridad de la organización. Los ingenieros de detección escriben reglas Sigma utilizando el lenguaje de consulta Sigma, que les permite expresar una lógica de detección compleja de una manera clara y eficiente.

‍

**¿Cómo facilita el convertidor Sigma la integración de las reglas Sigma con diferentes herramientas y plataformas de seguridad?**

El convertidor Sigma traduce las reglas Sigma a lenguajes de consulta o formatos específicos compatibles con diversas herramientas y plataformas de seguridad, como Elasticsearch, Splunk, ArcSight y QRadar. Esto permite a las organizaciones utilizar las reglas Sigma con su infraestructura de seguridad existente sin necesidad de realizar una conversión manual.

‍

**¿Qué papel juega el repositorio de reglas de Sigma en el ecosistema de Sigma?**

El repositorio de reglas de Sigma funciona como un repositorio centralizado para almacenar y compartir las reglas de Sigma aportadas por la comunidad. Proporciona un recurso valioso para que los ingenieros de detección accedan, descarguen y contribuyan a una biblioteca en crecimiento de contenido de detección que cubre una amplia gama de amenazas de seguridad y casos de uso.

‍

## **Preguntas de la entrevista sobre respuesta a incidentes relacionados con YARA:**

### **¿Qué es YARA y cómo se utiliza en ciberseguridad?**

YARA es una herramienta de búsqueda de patrones de código abierto que se utiliza principalmente en la investigación y detección de malware. Permite a los analistas crear reglas (firmas) para identificar y clasificar malware en función de características o patrones específicos que se encuentren en archivos o en la memoria.

‍

### **¿En qué se diferencia YARA de otras técnicas de detección de malware?**

YARA se diferencia de otras técnicas de detección de malware, como el software antivirus, al proporcionar a los analistas un marco flexible y personalizable para crear y compartir reglas de detección. Las reglas de YARA pueden apuntar a atributos o comportamientos específicos del malware, lo que las hace muy adaptables a las amenazas en evolución.

‍

### **¿Qué tipos de características de malware se pueden detectar utilizando las reglas YARA?**

Las reglas de YARA pueden detectar varias características de malware, incluidas cadenas específicas o secuencias de bytes, metadatos de archivos (por ejemplo, tamaño de archivo, tipo de archivo), patrones de código (por ejemplo, firmas de funciones) e indicadores de comportamiento (por ejemplo, patrones de comunicación de red, llamadas del sistema).

‍

**¿Cómo pueden los ingenieros de detección contribuir a la comunidad YARA?**

Los ingenieros de detección pueden contribuir a la comunidad YARA creando y compartiendo reglas YARA para detectar amenazas de malware nuevas o emergentes, probando y validando reglas existentes, brindando comentarios y mejoras a la sintaxis YARA y contribuyendo al desarrollo de herramientas y utilidades para trabajar con reglas YARA.

‍

### **¿Cómo contribuyen las reglas YARA a la respuesta a incidentes y a las investigaciones forenses?**

Las reglas de YARA desempeñan un papel importante en la respuesta a incidentes y en las investigaciones forenses, ya que ayudan a los analistas a identificar y clasificar los artefactos de malware presentes en los sistemas comprometidos. Los analistas pueden utilizar las reglas de YARA para buscar muestras de malware conocidas o indicadores de compromiso (IOC) específicos en grandes conjuntos de datos, lo que proporciona información valiosa sobre el alcance y el impacto de los incidentes de seguridad.

‍

**¿Qué papel juega YARA en la respuesta a incidentes y las investigaciones forenses?**

YARA puede desempeñar un papel importante en la respuesta a incidentes y en las investigaciones forenses, ya que ayuda a los analistas a identificar y clasificar los artefactos de malware presentes en los sistemas comprometidos. Las reglas de YARA se pueden utilizar para buscar muestras de malware conocidas o indicadores de compromiso (IOC) específicos en grandes conjuntos de datos.

‍

## **Preguntas de la entrevista para ingenieros de detección relacionados con Snort**

### **¿Cuál es el propósito de las reglas de Snort en la seguridad de la red y cómo contribuyen a la detección de amenazas?**

Las reglas de Snort son componentes esenciales del sistema de detección de intrusiones (IDS) y del sistema de prevención de intrusiones (IPS) de Snort. Estas reglas definen patrones o firmas específicos que Snort utiliza para detectar actividad potencialmente maliciosa en el tráfico de la red. Al comparar los paquetes con estas reglas, Snort puede identificar y alertar sobre varios tipos de amenazas basadas en la red, como escaneos de puertos, exploits y comunicación de malware.

‍

### **¿Cómo se estructuran las reglas de Snort y cuáles son los componentes principales de una regla de Snort?**

Las reglas de Snort constan de dos componentes principales: el encabezado de la regla y las opciones de la regla. El encabezado de la regla especifica la acción (alerta, registro, eliminación), el protocolo (TCP, UDP), las direcciones IP de origen y destino y los números de puerto. Las opciones de la regla definen los criterios para hacer coincidir el tráfico, como los patrones de contenido, los desplazamientos de bytes y los metadatos.

‍

### **¿Qué papel juegan los conjuntos de reglas de Snort en la ingeniería de detección?**

Los ingenieros de detección aprovechan estos conjuntos de reglas como base para sus estrategias de detección, personalizando y ajustando los conjuntos de reglas para que coincidan con los requisitos de seguridad únicos de la organización y el panorama de amenazas.

‍

**¿Qué tipos de ataques de red se pueden detectar utilizando las reglas de Snort?**

Las reglas de Snort pueden detectar una amplia gama de ataques basados ​​en la red, incluidos:

- Exploraciones de puertos y actividades de reconocimiento
- Intentos de explotación dirigidos a servicios vulnerables
- Comunicación de malware y tráfico de comando y control
- Ataques de denegación de servicio (DoS) y abuso de la red

‍

## **Referencias**

- https://letsdefend.io/blog/detection-engineer-interview-questions-and-answers
- [Awesome Detection Engineering - GitHub](https://github.com/infosecB/awesome-detection-engineering) : este es un repositorio dedicado a la ingeniería de detección. Proporciona una lista completa de conceptos, marcos, contenido de detección, firmas, registro, monitoreo y fuentes de datos.

- Establecer un programa de ingeniería de detección desde cero: este artículo proporciona una perspectiva sobre cómo establecer un programa de ingeniería de detección de manera eficaz y eficiente con los recursos disponibles2.

- Explicación de la ingeniería de detección | Splunk: este artículo explica qué es la ingeniería de detección y su importancia en el diseño, la construcción y el ajuste de sistemas y procesos para detectar actividades maliciosas o comportamientos no autorizados.

- [Matriz de madurez de ingeniería de detección | Kyle Bailey]: Esta es una matriz detallada que sirve como herramienta para medir la madurez general del programa de ingeniería de detección de una organización.

- [Modelo de nivel de madurez de detección (DML) | Ryan Stillions]: Este modelo define y describe 8 niveles diferentes de madurez del programa de detección de amenazas de una organización.

- [La Pirámide del Dolor | David J Bianco]: Un modelo utilizado para describir varias categorizaciones de indicadores de compromiso y su nivel de efectividad en la detección de actores de amenazas.

- [Cyber ​​Kill Chain | Lockheed Martin]: Marco de Lockheed Martin que describe las 7 etapas que se observan comúnmente en un ciberataque.

- [Modelo de definición de casos de uso MaGMa (Gestión, Crecimiento, Métricas y Evaluación)]: Un enfoque centrado en el negocio para definir casos de uso de detección de amenazas.

- [Objetos de registro adversarial sintético (SALO) | Splunk]: SALO es un marco para la generación de eventos de registro sin la necesidad de infraestructura o acciones para iniciar el evento que causa un evento de registro.

- [El zen de las reglas de seguridad | Justin Ibarra]: Este libro describe 19 aforismos que sirven como principios universales para la creación de contenido de detección de alta calidad.