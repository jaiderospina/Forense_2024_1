CLOUD COMPUTING


La definición de la Computación en la Nube según el Instituto Nacional de Estándares y Tecnología (NIST) describe un modelo que facilita el acceso a una red de manera ubicua, conveniente y bajo demanda, a un conjunto compartido de recursos informáticos configurables. Estos recursos pueden incluir redes, servidores, almacenamiento, aplicaciones y servicios, los cuales pueden ser provisionados y lanzados con un mínimo esfuerzo de gestión o interacción con el proveedor de servicios. Este modelo de nube se caracteriza por cinco elementos esenciales: acceso bajo demanda a recursos, amplio acceso a la red, agrupación de recursos, elasticidad rápida y servicio medido. Además, se compone de tres modelos de servicio: Software como Servicio (SaaS), Plataforma como Servicio (PaaS) e Infraestructura como Servicio (IaaS); y cuatro modelos de implementación: nube pública, nube privada, nube comunitaria y nube híbrida.


Las características esenciales de la computación en la nube son:
* Autoservicio bajo demanda: Los consumidores pueden obtener capacidades informáticas de forma automática y sin necesidad de interacción humana con el proveedor de servicios. Pueden suministrar unilateralmente recursos como tiempo de servidor y almacenamiento según lo necesiten
* Amplio acceso a la red: Las capacidades de la nube están disponibles a través de la red y se accede a ellas mediante mecanismos estándar que promueven su uso en una variedad de dispositivos, desde teléfonos móviles hasta estaciones de trabajo.
* Agrupación de recursos: Los recursos informáticos del proveedor se agrupan para servir a múltiples consumidores en un modelo multi inquilino. Estos recursos, físicos y virtuales, se asignan y reasignan dinámicamente según la demanda del consumidor, lo que proporciona una sensación de independencia de ubicación para el cliente.
* Elasticidad rápida: Las capacidades de la nube pueden aprovisionarse y liberarse elásticamente, escalando rápidamente hacia afuera y hacia adentro según la demanda. Esto brinda a los consumidores la sensación de que las capacidades disponibles son ilimitadas y pueden ser apropiadas en cualquier cantidad en cualquier momento.
* Servicio medido: Los sistemas en la nube controlan y optimizan automáticamente el uso de recursos, utilizando una capacidad de medición adecuada para el tipo de servicio. Se monitorea, controla y reporta el uso de recursos, brindando transparencia tanto para el proveedor como para el consumidor del servicio utilizado.


Los modelos de servicio de computación en la nube incluyen:
* Software como servicio (SaaS): Permite al consumidor utilizar aplicaciones del proveedor que se ejecutan en la infraestructura de la nube. Estas aplicaciones son accesibles desde varios dispositivos cliente a través de una interfaz ligera, como un navegador web. El consumidor no administra la infraestructura subyacente, incluida la red, los servidores o el almacenamiento, excepto ciertos ajustes de configuración.
* Plataforma como servicio (PaaS): Permite al consumidor implementar en la infraestructura de la nube aplicaciones creadas o adquiridas por él mismo, utilizando lenguajes de programación, bibliotecas, servicios y herramientas compatibles con el proveedor. El consumidor no gestiona la infraestructura subyacente, pero tiene control sobre las aplicaciones implementadas y posiblemente sobre los ajustes de configuración para el entorno de alojamiento de aplicaciones.
* Infraestructura como servicio (IaaS): Permite al consumidor proporcionar procesamiento, almacenamiento, redes y otros recursos informáticos fundamentales, donde puede implementar y ejecutar software arbitrario, incluyendo sistemas operativos y aplicaciones. El consumidor no gestiona la infraestructura subyacente, pero tiene control sobre los sistemas operativos, el almacenamiento y las aplicaciones implementadas, y posiblemente sobre componentes de red seleccionados, como firewalls de host.


Los modelos de implementación en la nube son: 
* Nube privada: La infraestructura de la nube se proporciona para el uso exclusivo de una única organización, que puede ser propiedad de, administrada y operada por la organización misma, un tercero o una combinación de ambos. Puede estar ubicada dentro o fuera de las instalaciones de la organización.
* Nube comunitaria: La infraestructura de la nube se proporciona para el uso exclusivo de una comunidad específica de consumidores de organizaciones que comparten intereses, como requisitos de seguridad o consideraciones de cumplimiento. Puede ser propiedad de, administrada y operada por una o más organizaciones de la comunidad, un tercero o una combinación de ambos, y puede estar dentro o fuera de las instalaciones.
* Nube pública: La infraestructura de la nube está disponible para su uso abierto por el público en general y puede ser propiedad de, administrada y operada por una organización empresarial, académica o gubernamental, o una combinación de ellas. Por lo general, está ubicada en las instalaciones del proveedor de la nube.
* Nube híbrida: Es una composición de dos o más infraestructuras de nube distintas (privada, comunitaria o pública) que siguen siendo entidades únicas, pero están interconectadas mediante tecnología estandarizada o patentada que permite la portabilidad de datos y aplicaciones, como la explosión de nubes para equilibrar la carga entre ellas.


La virtualización es un proceso clave en la computación en la nube que implica la creación de máquinas virtuales (VM), implementaciones de software que simulan computadoras físicas y sus entornos. Estas VM se separan de sus recursos subyacentes mediante un contenedor de ejecución, como un sistema operativo o un programa. La virtualización se aplica en diversas áreas, como servidores, almacenamiento y redes, y puede enmascarar la complejidad, permitiendo el uso compartido y la utilización eficiente de recursos.
El hipervisor es esencial para el funcionamiento de las VM, ya que actúa como el hardware subyacente ante la VM. Sin embargo, el hipervisor también puede ser un punto vulnerable, ya que es un programa de software y su compromiso puede plantear riesgos de seguridad significativos. Si el hipervisor se ve comprometido, puede poner en peligro tanto las VM como la máquina host, ya que tiene un alto nivel de control sobre el sistema. Por lo tanto, la seguridad del hipervisor es crucial para garantizar la integridad y la seguridad de las VM y del entorno de virtualización en general.


Existen varios tipos de virtualización:
* Nativa o básica: Utiliza un hipervisor que se ejecuta directamente en el hardware básico. Los sistemas operativos invitados se ejecutan sobre este hipervisor. Ejemplos incluyen Microsoft Hyper-V, Oracle VM, VMware ESX, entre otros.
* Virtualización alojada: Utiliza un hipervisor que se ejecuta como una aplicación dentro de un sistema operativo host. Las máquinas virtuales se ejecutan sobre este hipervisor. Ejemplos son Oracle VirtualBox, VMware Server, Xen, entre otros.
* Virtualización implementada por el sistema operativo: Es implementada por el propio sistema operativo en lugar del hipervisor. Ejemplos incluyen Solaris Containers, BSDjails, Linux-VServer, entre otros.


La ciencia forense digital implica la aplicación de la informática y procedimientos de investigación para examinar evidencia digital, asegurando la autoridad de búsqueda, la cadena de custodia, la validación con matemáticas, el uso de herramientas validadas, la repetibilidad, la generación de informes y, posiblemente, la evaluación experta. Una definición alternativa describe la ciencia forense digital como la aplicación de la ciencia para identificar, recopilar, examinar y analizar datos, mientras se preserva la integridad de la información y se mantiene una estricta cadena de custodia para los datos.
La ciencia forense digital, según la definición de Palmer en el Taller de Investigación Forense Digital (DFRWS), implica el uso de métodos científicamente probados para preservar, recopilar, validar, identificar, analizar, interpretar y presentar evidencia digital con el propósito de reconstruir eventos criminales o prevenir acciones no autorizadas perjudiciales. La necesidad de una metodología estructurada para investigar delitos informáticos llevó al desarrollo de la ciencia forense digital. En 1984, el FBI y otras agencias de aplicación de la ley desarrollaron enfoques para recopilar y analizar evidencia informática, lo que condujo a la creación del Equipo de Respuesta y Análisis Computarizado (CART) para este propósito.
El FBI convoca conferencias internacionales en 1995, 1996 y 1997 para establecer estándares en la ciencia forense informática, resultando en la formación del Grupo de Trabajo Científico sobre Evidencia Digital (SWGDE). En 1998, el Instituto Nacional de Justicia (NIJ) de Estados Unidos creó el Grupo de Trabajo Técnico para la Investigación Electrónica de la Escena del Crimen (TWGECSI) con la tarea de establecer criterios para investigaciones electrónicas. Este grupo, compuesto por expertos de diversas áreas, publicó en 2001 la "Guía para socorristas" sobre investigación electrónica de la escena del crimen. Este documento, parte de una serie sobre métodos forenses digitales, define la evidencia digital como información de valor almacenada, recibida o transmitida a través de dispositivos electrónicos.
La evidencia digital adquirida durante el aseguramiento de datos o dispositivos electrónicos tiene características particulares: es latente (como huellas dactilares o evidencia de ADN), puede cruzar fronteras jurisdiccionales fácilmente, es susceptible de alteración o destrucción y puede requerir una respuesta urgente.
Antes de recolectar pruebas en la escena de un crimen, es crucial asegurar la autoridad legal para confiscar pruebas, documentar y asegurar la escena, y utilizar el equipo de protección personal adecuado.
La guía recomienda los siguientes pasos para el manejo de evidencia digital en la escena del crimen electrónico: reconocer, identificar, incautar y proteger toda la evidencia digital, documentar la escena y la ubicación específica de la evidencia, recopilar, etiquetar y preservar la evidencia digital, y empacar y transportarla de manera segura.
Además, la guía enfatiza que el acceso inadecuado a los datos almacenados en dispositivos electrónicos puede violar las leyes federales, por lo que los investigadores pueden necesitar obtener autoridad legal adicional antes de continuar.


Leyes y directrices relevantes:
* La ley de Política de Comunicaciones por Cable permite el uso discrecional de Información Personal Identificable (PII) por parte de los operadores de cable, pero restringe su divulgación a terceros.
* La ley de Protección de la Privacidad Infantil en Línea (COPPA) busca proteger a los niños menores de 13 años en línea.
* Las reglas de Información de Red de Propiedad Intelectual del Cliente aplican restricciones al uso de información del cliente tanto internamente como con terceros, especialmente a las compañías telefónicas.
* La ley de privacidad de las comunicaciones electrónicas protege la información intercambiada para evitar su interceptación o divulgación por terceros, incluidas las fuerzas del orden.


El código de Prácticas Justas de Información de los Estados Unidos de 1973 establece:
* La transparencia en la existencia de sistemas de mantenimiento de registros de datos personales.
* El derecho de las personas a conocer qué información sobre ellas se encuentra en un registro y cómo se utiliza.
* El derecho de las personas a evitar que la información sobre ellas, obtenida para un propósito, se utilice o divulgue para otros propósitos sin su consentimiento.
* La responsabilidad de las organizaciones que manejan registros de identificación de datos personales para garantizar la fiabilidad de los datos y tomar precauciones para evitar su uso indebido.


La Unión Europea (UE) establece principios de privacidad que incluyen:
* Limitación de la divulgación de información sobre un individuo a menos que esté autorizada por la ley o el consentimiento del individuo.
* Recopilación de datos de acuerdo con la ley.
* Mantenimiento de registros precisos y actualizados sobre un individuo.
* Derecho de las personas a corregir errores en sus datos personales.
* Uso de los datos sólo para los fines para los que fueron recopilados y durante un período razonable.
* Derecho de las personas a recibir un informe sobre la información que se tiene sobre ellas.
* Prohibición de la transmisión de información personal a lugares donde la protección de datos equivalente no pueda garantizarse.


La Organización para la Cooperación y el Desarrollo Económicos (OCDE) ha emitido directrices que incluyen:
* Establecimiento de límites a la recopilación de datos personales, obtenidos de manera legal y justa.
* Garantía de que los datos personales sean relevantes, precisos, completos y se mantengan actualizados para los fines previstos.
* Especificación clara de los fines para los cuales se recopilan los datos personales en el momento de la recopilación.
* Prohibición de la divulgación o uso de datos personales para fines distintos a los especificados.
* Protección de los datos personales mediante salvaguardias de seguridad informática contra riesgos como pérdida, acceso no autorizado, destrucción, uso, modificación o divulgación.
* Fomento de una política de transparencia sobre el manejo de datos personales.
* Garantía de que un individuo tenga derecho a obtener información de un controlador de datos.
* Abstención de restringir los flujos transfronterizos de datos personales entre países miembros, excepto en circunstancias específicas.
* Posibilidad de imponer restricciones respecto a ciertas categorías de datos personales si la legislación nacional sobre privacidad incluye principios específicos y el otro país miembro no proporciona una protección equivalente.


La ciencia forense de la computación en la nube, según el NIST, se define como la aplicación de principios científicos y tecnológicos para reconstruir eventos pasados en la nube mediante la identificación, recopilación, preservación, examen, interpretación y presentación de evidencia digital. Ruan et al. proponen un modelo tridimensional que estructura este dominio, que incluye una dimensión técnica, organizacional y legal.


La dimensión técnica de la ciencia forense de la nube abarca diversas actividades, como la recopilación de datos, el análisis forense en vivo, la segregación de evidencia, los entornos virtualizados y las medidas proactivas. La recopilación de datos implica la identificación, etiquetado, registro y adquisición de datos forenses, tanto del lado del cliente como del proveedor. Es crucial preservar la integridad de los datos y respetar las leyes y regulaciones pertinentes, así como la confidencialidad de otros inquilinos de la nube.


Consideraciones técnicas:
* La necesidad de herramientas forenses que permitan la adquisición, recuperación, examen y análisis de datos en entornos de nube elásticos y dinámicos.
* El desarrollo de procedimientos y herramientas para la segregación adecuada de datos entre múltiples inquilinos y modelos de implementación de nube.
* La falta de procedimientos de investigación del hipervisor en relación con la virtualización en la nube.
* La importancia de desarrollar métodos para la localización precisa de datos forenses, considerando las marcas de tiempo y las cuestiones jurisdiccionales.
* La implementación de medidas proactivas, como la conservación de instantáneas de almacenamiento, el seguimiento continuo de la autenticación y el control de acceso, así como auditorías detalladas de todos los accesos, para mejorar el proceso de investigación.


El NIST destaca preocupaciones adicionales sobre la dimensión técnica de la ciencia forense en la nube, señalando que la identificación, recopilación y preservación de medios pueden ser desafiantes debido a los siguientes factores:
* Identificar al proveedor de la nube y sus asociados.
* Identificar las cuentas adecuadas mantenidas por el consumidor en la nube.
* Obtener acceso a los medios deseados.
* Obtener asistencia del personal del proveedor de la nube.
* Comprender la topología y políticas de propiedad de la nube.
* Obtener una imagen forense completa de los medios una vez que se obtiene el acceso.
* Manejar el gran volumen de medios.
* Responder a ubicaciones físicas múltiples si es necesario.
* Lidiar con el descubrimiento electrónico y los derechos de privacidad en un entorno multi inquilino.
* Validar la imagen forense.
* Realizar análisis de datos cifrados y obtener claves de cifrado.
* Adaptarse al almacenamiento no localizado.
* Lidiar con la falta de asociación directa entre las pruebas y un sospechoso específico, confiando en la información proporcionada por el proveedor de la nube.


Las herramientas forenses digitales tradicionales han evolucionado para adaptarse al análisis forense en la nube. 
Algunas de las más populares incluyen:
* Access Data Forensic Toolkit (FTK)
* EnCase
* F-Response
* Internet Evidence Finder (IEF) de Magnet Forensics


La dimensión organizacional en el análisis forense en la nube implica la cooperación entre auditores, operadores, agentes de nube, consumidores y proveedores para obtener evidencia digital. Para establecer una capacidad forense en la nube, cada entidad debe proporcionar personal interno y colaborar entre proveedor y cliente, desempeñando roles clave:
* Investigadores
* Profesionales de TI
* Controladores de incidentes
* Asesores legales
* Asistencia externa


La dimensión jurídica del análisis forense en la nube implica el desarrollo de regulaciones y acuerdos para asegurar el cumplimiento legal y proteger la confidencialidad de los datos. Los SLA deben definir los términos de uso entre el proveedor de servicios en la nube (CSP) y sus clientes, incluyendo aspectos relacionados con las investigaciones forenses. Estos términos deben abordar los servicios prestados, los límites de confianza, los procesos para realizar investigaciones en entornos multijurisdiccionales, la medición de la efectividad de la resolución de incidentes, el tiempo de entrega de datos, el método de autenticación para investigadores y el tipo de datos a recopilar.
Al establecer una capacidad forense en la nube, es crucial considerar aspectos adicionales que abarcan las dimensiones técnicas, organizativas y legales.
* Recolección de datos forenses
* Análisis forense estático, elástico y en vivo
* Segregación de evidencia
* Múltiples copias de datos
* Ambientes virtualizados
* Personal interno
* Cadenas de dependencia externa
* Acuerdos de Nivel de Servicio
* Múltiples jurisdicciones y arrendamiento


Retos identificados por NIST:
* Arquitectura
* Recolección de datos
* Sistemas informáticos locales
* Clasificación forense
* Análisis forense como servicio (FaaS)
* Técnicas anti forenses
* Entrenamiento constante


Los modelos forenses digitales son marcos estructurados que guían el proceso de investigación forense en el ámbito digital. Aquí se presentan varios modelos:
Consta de nueve etapas, incluyendo identificación, preparación, preservación, examen, entre otras.


* Modelo de Procesos de Evidencia Forense Digital: Define etapas como identificación, recolección, análisis e interpretación, y presentación.
* Modelo DFRWS: Define procesos como identificación, preservación, recolección, examen, análisis y presentación.
* Modelo Ampliado de Investigaciones de Delitos Cibernéticos: Describe el flujo de información e incluye actividades como concientización, búsqueda de pruebas y presentación de pruebas.
* Modelo Armonizado de Procesos de Investigación Forense Digital: Es iterativo y abarca desde la detección de incidentes hasta la conclusión, pasando por la identificación, recopilación y análisis de evidencia.
* Proceso Integrado de Investigación Digital (IDIP): Se divide en grupos como preparación, investigación física y digital de la escena del crimen, y revisión.
* Modelo IDIP Mejorado: Agrega fases adicionales como rastreo y dinamita para identificar dispositivos y adquirir evidencia adicional.
* Modelo Sistemático de Investigación Forense Digital: Se centra en fases como preparación, aseguramiento de la escena, recolección de evidencia, análisis y presentación.


El proceso de investigaciones forenses en la nube se puede dividir en cuatro pasos:
* Determinar el propósito de la investigación.
* Identificar los tipos de servicios en la nube.
* Seleccionar el tipo de tecnología a aplicar.
* Inspeccionar las ubicaciones físicas y lógicas.


El Proceso Forense en la Nube enfatiza la admisibilidad de la evidencia a través de las siguientes cuatro fases:
* Identificar el propósito de la investigación.
* Determinar el tipo de servicio en la nube.
* Determinar el tipo de tecnología en la nube.
* Realizar la investigación.


El Modelo Avanzado de Adquisición de Datos comprende tres etapas: 
* Planificación inicial, levantamiento en sitio y adquisición de datos electrónicos.


El Marco Forense Digital Conceptual Integrado para la Computación en la Nube se enfoca en las cuatro etapas: 
* Identificación y preservación, recopilación, examen y análisis, e informes y presentación.


El Modelo Integrado de Proceso Forense Digital es un modelo integral que abarca las siguientes etapas: 
* Preparación, incidentes, respuesta a incidentes, investigación física, investigación digital, presentación y documentación.


El Modelo Forense de Nube Abierta comprende las siguientes etapas: 
* Preservación, identificación, recopilación, organización, presentación y verificación.


El modelo de madurez de capacidades forenses en la nube (CMM), desarrollado por Cloud Security Alliance, es utilizado por consumidores y proveedores de servicios en la nube para evaluar la madurez de sus procesos para realizar investigaciones forenses digitales en el entorno de la nube.


El modelo se basó en el Marco de Madurez de Procesos de Software (SEI) del Instituto de Ingeniería de Software de la Universidad Carnegie Mellon, que identifica cinco niveles progresivos de madurez de procesos:
* Inicial – ¿Cómo vamos a hacer esto?
* Repetible – ¿Hemos hecho esto alguna vez antes?
* Definido – ¿Cuál es nuestro proceso para hacer esto?
* Gestionado – ¿Qué recursos requirió esto?
* Optimización – ¿Cómo podemos hacerlo mejor?


El modelo SEI se aplica al análisis forense de la nube para proporcionar orientación de alto nivel por nivel, centrándose inicialmente en el uso de la nube IaaS.
