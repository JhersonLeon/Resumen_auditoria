 
 

 

Tema: 

Auditoria al centro de operaciones de Seguridad (SOC) 

  

Docente: 

  

Mg. Ivan Vladimir Martinez Moran 

  

Integrantes: 

 

Leon Tito, Jherson Estefano 

Talavera Urbano Amer 

Arias Bautista Kimberli Rosio 

Melendez Guadalupe Helder 

Text Box 

 
  

  

 
 

 

 

 

Lima, Perú 

 

 

Estructura del Trabajo de Auditoría Informática 

  

Introducción  

 	 En la actualidad, la seguridad de la información se encuentra involucrado en diversas áreas dentro de una empresa, ya que poseen una gran cantidad de información, lo cual no puede ser vulnerada por alguna persona. De esta manera, para evitar incidentes se crearon áreas de trabajo que estén respaldando y monitoreando constantemente la información con la finalidad de evitar pérdidas masivas de datos que perjudiquen tanto a la empresa como a las personas que forman parte de ella. 

De este modo, ante diversos ataques que se dieron a conocer, muchas empresas optaron por un Centro de Operaciones de Seguridad (SOC), para garantizar la seguridad de la información. 

 

Definición del problema   
 

En el área de centro de operaciones de seguridad (SOC) de la empresa Netsecure SAC se han evidenciado problemas en el cumplimiento de las notificaciones de eventos y alertas hacia los usuarios finales, los cuales son generadas por las herramientas de monitoreo y correlación de eventos. 

En el área de centro de operaciones de seguridad (SOC) de la empresa Netsecure SAC se ha evidenciado diferentes problemas. A continuación, se detallan cada una de ellas, en primer lugar, se ha encontrado deficiencias en el cumplimiento los procesos de las notificaciones de eventos y alertas hacia los usuarios finales, los cuales son generadas por las herramientas de monitoreo y correlación de eventos. En segundo lugar, existe problemas con la herramienta SIEM, el cual es el encargado de recopilar todas las alertas provenientes de otras aplicaciones, el problema se encuentra que hay algunas alertas no contienen toda la información dentro del payload, por lo tanto, el proceso de gestión de incidencias se hace más lenta generando un sobrecargo de alertas, por último, los analistas no cumplen con los procesos y procedimientos a la hora de gestionar las incidencias  

 

 

 

Selección Empresa Para Auditar  

NetSecure SAC 

 

Introducción al caso de Auditoria (Proceso/Área) 

NetSecure es una empresa dedica a brindar servicios de seguridad de la información, es por lo que se ha implementado el área de centro de operaciones de seguridad (SOC) que se encarga de la supervisión y administración de seguridad de la información de sus clientes, utilizando herramientas de monitoreo y correlación de eventos. Esta área se encarga de gestionar las alertas e incidencias generadas por las herramientas, que permiten un adecuado monitoreo en tiempo real del comportamiento de los equipos finales (servidores, Firewalls, etc) donde los analistas de seguridad son los responsables de evaluar y tomar acciones necesarias sobre las notificaciones emitidas con la finalidad de prevenir posibles incidencias que puedan afectar la continuidad del negocio. 

 

2. Definición del Problema 

2.1. Planteamiento del Problema 

La empresa NetSecure en los últimos años ha experimentado problemas en cuanto a la gestión de casos, flujos de trabajo y la organización de tareas; a la fecha cuenta con una solución SIEM que recepcioná los eventos y lo correlaciona, para luego ser gestionados y supervisados por la herramienta SOAR que genera alertas y respuestas automáticas según sea necesario. Estas alertas son enviadas al área de SOC, donde los analistas son los encargados de revisar y dar aviso al cliente sobre el caso encontrado, sin embargo, estas alertas son enviados con un retraso de 1 a 2 horas aproximadamente lo cual incumple los SLA estipulado en el contrato. 

Asimismo, se evidenció algunas falencias en la misma solución (SIEM) de que algunos eventos no son procesados y correlacionados correctamente, debido a ello se genera alertas tipo falsos positivos.  

Por lo tanto, esta problemática está impactando directamente a sus clientes y a la misma empresa, ya que se está incumpliendo con los acuerdos de nivel de servicio (SLA), de modo que la empresa corre el riesgo de pérdida de clientes. 

 

2.2. Formulación del Problema 

Los clientes de la empresa NetSecure han mostrado su inconformidad por algunas alertas que han recibido, que son de tipo falsos positivos que la herramienta de monitoreo generó, las cuales son acciones que son provocadas por los mismos trabajadores de la empresa dentro de la red, como muchos intentos de logeos fallidos de un usuario autorizado a un servidor, conexiones de una sola IP origen hacia diferentes servidores, todas estas acciones son parte del día a día de trabajo. Así mismo, se han visto perjudicados por algunas alertas enviadas por el sistema, ya que la información llega incompleta en el payload y esto genera un retraso en el tiempo de respuesta sobre el incidente o amenaza. 

Por lo tanto, se evaluará el nivel de cumplimiento de las normas y a cerca de los factores que están afectando la eficiencia y la eficacia del SOC para realizar una adecuada detección, respuesta y mitigación de incidentes de seguridad. 

 

2.3 Definición del Proceso a auditar 

Control y administración de eventos en el área de SOC. 

En este proceso se auditará al personal analista de seguridad, desarrollo de sus funciones y los roles que cumplen para llevar a cabo los trabajos de análisis y tratamiento de las alertas en base a las herramientas de gestión y administración de eventos.  

Se verificará el proceso de gestión de eventos, análisis, identificación y recuperación de información. Asimismo, las alertas son analizadas por los especialistas de seguridad, para ser reenviadas a los clientes con el fin de verificar y determinar, si se debe tomar acciones preventivas o correctivas.  

Finalmente se realizará la verificación de la recepción de datos en la herramienta de correlación de eventos, como la calidad de información almacenada en el mismo para luego ser identificada y clasificada según su tipo (amenaza, ataque o vulnerabilidad). 

 

3. Marco Referencia 

3.1. Marco Contextual 

3.1.1. Datos de la Empresa	 

NetSecure S.A.C  
RUC: 2052107101		 

3.1.2. Misión 

Enfocados en ofrecer soluciones altamente competitivas, que contribuyan al desarrollo sostenible y ayudar a las empresas en el complejo camino de la ciberseguridad; en el análisis, detección y prevención de amenazas digitales. 

3.1.3. Visión 

Comprometidos con los problemas de nuestros clientes de forma transparente y eficaz para convertirnos en su Socio de confianza y construir un mundo digital más seguro. 

 

3.1.4. Organigrama 

 

3.1.5. Topología de la Red 

 	 

3.1.6. Seguridad del área  

Para mantener la seguridad del área la empresa NetSecure cuenta con equipos electrónicos asignados al área de SOC y a cada personal responsable para ejecutar las tareas, por otro lado, las conexiones remotas hacia los servidores están permitidos únicamente a través de la VPN de la empresa.  

Los administradores de infraestructura de TI son los principales responsables de supervisar y controlar los accesos a las herramientas de monitoreo y correlación de eventos, es por ello todos los accesos a estas herramientas y servidores están basados por roles. Asimismo, la ejecución de tareas por los analistas y especialistas están basados por roles y funciones asignados. 

Por último, la concientización del personal es un punto muy importante para afianzar la seguridad de la organización para poder resguardar la confidencialidad e integridad de la información. 

 

3.1.7. Procedimientos 

El área de Centro de Operaciones de Seguridad (SOC), se encarga de realizar un seguimiento continuo y análisis de la actividad en redes, servidores, equipos finales, bases de datos, aplicaciones y otros sistemas; buscando actividades anómalas y sospechosas que pueden ser indicativos de un incidente, posibles amenazas o ataques. Para poder garantizar la seguridad de la información, el área de SOC está conformado por niveles en función, según el grado de especialización de los analistas y cada uno sigue un procedimiento específico. 

Nivel 1, están conformados por analistas capacitados, que  se encargan de recepcionar las alertas emitidas por la herramienta SOAR, luego evalúan estas alertas de seguridad si estas han sido emitidos correctamente con los datos completos y necesarios, para poder constatar ello el analista debe ingresar a la herramienta SIEM con los credenciales asignados; una vez dentro debe validar la ofensa registrada a que tipo de tecnología corresponde, tipo de actividad y la clasificación de nivel de riesgo; tras constatar que la información es correcta la alerta debe ser  derivarlo a los analistas de nivel 2. 

Nivel 2, los analistas son encargados de verificar y analizar la alerta a detalle, para luego determinar si los datos o el sistema se han visto afectados o comprometidos, tras haber determinado y clasificado, se emite una respuesta al cliente con la recomendación necesaria para que puedan tomar acciones preventivas o correctivas al respecto.   

Finalmente, se espera algún feedback por el lado del cliente, de requerir algún cambio o ajuste en el caso de uso, como por ejemplo ajustes en el umbral, la lógica, excepciones de usuarios e IP’s permitidas y de ser necesario se debe generar un nuevo caso de uso que pueda cumplir con los requerimientos específicos. 

 

4. Desarrollo de la Auditoría 

4.1. Fase 1 – Elaboración del Plan de Auditoría 

4.1.1. Objetivos 

4.1.1.1. Objetivo General 

Nuestro objetivo general es realizar una auditoría al área de Centro de Operaciones de Seguridad (SOC) en la empresa NetSecure SAC, con la finalidad de evaluar si los sistemas implementados y procesos de gestión de la información cumplen con las políticas y estándares específicos de TI. 

 

4.1.1.2. Objetivos Específicos 

Identificar las herramientas implementadas para la gestión de eventos y la eficiencia de estos. 

Evaluar si los eventos registrados son legibles y válidos para ser procesados por la herramienta. 

Evaluar los procesos y procedimientos de la gestión de información en el SOC. 

Identificar los riesgos asociados a los sistemas implementados y brindar métodos para mitigarlo. 

Evaluar los procedimientos de contingencia de la herramienta SIEM ante una caída del principal. 

Evaluar el plan de acción de recuperación ante desastres (DR) de la herramienta SIEM. 

Evaluar si el área del SOC está cumpliendo con el SLA (acuerdo de nivel de servicio). 

4.1.1.3. Alcance 

La auditoría se realizará específicamente al centro de operaciones de seguridad SOC situado en Lima, Perú. En las cuales se evaluarán la eficiencia y eficacia de los sistemas implementados, los procesos y procedimientos que se realizan para la gestión de eventos recepcionados. Asimismo, se evaluará la calidad y legibilidad de los eventos registrados por la herramienta, esto se evaluará solamente la información almacenada dentro del periodo de retención definido, más no la información que están almacenadas fuera de la herramienta. Finalmente, se evaluará el plan de acción ante desastres, específicamente para las herramientas de correlación de eventos, más no de los otros sistemas del área. 

4.1.2. Plan de Auditoria 

4.1.2.1. Investigación Preliminar 

Según las validaciones realizadas, la empresa NetSecure realizó un inventariado en el año 2019 de los equipos finales asignados al área de operaciones, los cuales fueron proporcionados para la ejecución de las tareas y actividades diarias dentro de la organización. En este inventariado realizado obtuvieron las características de los equipos tanto de hardware como software y programas utilizados por los usuarios, dicho motivo fue identificar y contabilizar los equipos utilizados por la empresa y sus propiedades.  

4.1.2.2. Recolección de Información 

Encuestas 

Las encuestas son instrumentos muy usados para la recolección de información cualitativa y/o cuantitativa de una población. Para ello, se elabora un cuestionario, cuyos datos obtenidos será procesados con métodos estadísticos. Las encuestas son entonces una herramienta para conocer las características de un grupo de personas. 

Entrevista 

Las entrevistas son una herramienta fundamental para obtener un testimonio oral, a partir del cual se podrá reconstruir un suceso histórico, o explorar diferentes aspectos de una persona o un grupo. Las entrevistas pueden clasificarse en individuales o grupales, con el objetivo de obtener datos cualitativos observando las interacciones que se dan entre las personas. 

Revisión de registros existentes 

La revisión de registros tiene lugar cuando un investigador examina y extrae información de documentos que contienen datos sobre el participante. Los registros revisados en una investigación pueden ser públicos o privados. 

Pruebas 

Una prueba es una forma o una tarea física o mental para la cual se ha determinado un estándar normal, o para la cual se conoce las respuestas correctas. El desempeño de un participante en una prueba es comparado contra estos estándares y/o respuestas correctas. 

Observación 

La observación es uno de los métodos de recolección de datos más viables de implementar, ya que puede realizarse simplemente yendo al lugar en donde se dan naturalmente las situaciones que se buscan investigar. El investigador puede optar por la observación participante, en donde actúa de manera directa sobre los hechos, en donde se mantiene al margen de los hechos que ocurran. 

4.1.2.3. Aplicación de Instrumentos 

Para el caso de la auditoria planteada para el área de SOC, se utilizarán los siguientes instrumentos: 

Encuestas 

La aplicación de este instrumento ayudara a la recolección de información de la auditoria a realizar, debido que nos permite identificar riesgos potenciales, ya que las preguntas realizadas por este medio serán diseñadas para obtener información precisa sobre las políticas y procedimientos que se aplican en el área. Así mismo se puede obtener información de cómo se están ejecutando los controles internos en el área de SOC. Otro punto asertivo es que, por medio de las encuestas se pueden identificar las oportunidades de mejora tomando en cuenta la opinión de los empleados sobre cómo se puede mejorar el proceso de una actividad.  

En conclusión, las encuestas son claves para obtener información para una auditoria por que pueden obtener de una forma eficaz y eficiente de recopilar información de un proceso o empresa. 

 

Entrevistas 

Esta herramienta ayudara en la recopilación de información de primera mano directamente de las personas que laboran en el área de operaciones, el cual se obtendrá información acerca de los procesos y los controles que tienen definidos dentro de la empresa. 

4.1.2.4. Ejecución de Pruebas. 

4.1.2.5. Proceso de Análisis y Evaluación de Riesgos. 

Tras la información recopilada mediante las entrevistas y encuestas se ha identificado algunas posibles vulnerabilidades, amenazas y riegos que pueden causar algún impacto en la seguridad de la información de la organización y de sus clientes. 

Vulnerabilidad 

Parches de seguridad no actualizados en el área de operaciones	 

Falta de capacitación al personal del área de operaciones 

Gestión inadecuada de los roles de acceso en el área de operaciones 

Capacidad de licencia de EPS (Procesamiento de eventos por segunda limitada 

Amenazas 

Ciber-Ataque (Malware, DDoS, etc) 

Deficiencia en la gestión de la información y de las alertas. 

Accesos no autorizados a las herramientas de la seguridad de la información. 

Saturación de la herramienta SIEM y falla en el funcionamiento. 

Déficit en la actividad de red y actividad de registro de eventos en tiempo real.  

Riesgos 

Exposición de información de los clientes 

Incumplimiento en el SLA (contrato establecido entre proveedor y cliente) por la deficiencia en la gestión de las alertas. 

Pérdidas económicas y de la reputación de la empresa. 

Riesgo de la seguridad de la información. 

Pérdida y/o alteración de la información sensible. 

Eventos no recepcionados por la indisponibilidad de la herramienta. 

Eventos no procesados y recepcionados de manera correcta por la limitación de licencia de EPS. 

4.1.2.6. Tratamiento de Riesgo. 

Riesgo 

Tratamiento del riesgo 

Exposición de información 

Revisión de las actualizaciones de manera periódica por el área encargado de soporte para la prevención de robos de información y exposición de datos. 

Incumplimiento en el acuerdo de nivel de servicio (SLA) por la deficiencia en la gestión de las alertas. 

Elaborar métricas e indicadores para medir el índice de cumplimiento y rendimiento del SLA de manera periódica. 

Pérdidas económicas, clientes y de la reputación de la empresa. 

 

 

 
Riesgo de la seguridad de la información. 

 

 

 

 
Pérdida y/o alteración de la información sensible. 

Definir políticas y procedimientos para el tratamiento de la información de los clientes y de la misma organización. 

 

Elaborar un plan de capacitación constante para el personal del área de SOC y se debe definir los roles de acceso a las herramientas por cada especialista. 

 

Realizar copias de seguridad frecuentemente para respaldar la información sensible y almacenarla en ubicaciones seguras, como discos duros externos o servicios de almacenamiento en la nube. 

Eventos no recepcionados por la indisponibilidad de la herramienta. 

Verificación y monitoreo constante de recursos de los equipos para un adecuado funcionamiento y procesamiento de datos. 

Eventos no procesados y recepcionados de manera correcta por la limitación de licencia de eventos por segundo (EPS). 

Definir y establecer los límites claros relación con la cantidad de eventos que la herramienta puede procesar y recibir correctamente en función de la licencia adquirida. 

             

 

 

 

 

 

 

 

 

Text BoxText Box 

 

 

Semana 8 

4.1.2.7. Dictamen de la Auditoria 

Se ha realizado una auditoria al área de Centro de Operaciones de Seguridad (SOC) de la empresa NetSecure SAC. Esta auditoría se ha llevado a cabo con la finalidad de evaluar y obtener información detallada a cerca de los procesos, controles, análisis de la eficiencia de las herramientas de seguridad TI y verificación del cumplimiento de la normativa general de la empresa.  

Durante la auditoría realizada se ha identificado que la herramienta SIEM presenta deficiencias al momento de correlacionar los eventos debido a la saturación de recursos por el alto procesamiento de la información. Asimismo, se ha verificado que los eventos no están siendo procesados correctamente debido a la limitación de licencia, lo cual hace que algunos eventos no se procesen de manera correcta e incluso se dejan de recibir algunos eventos. Por otro lado, se ha evidenciado que hay parches de seguridad de los equipos que no están actualizados debidamente, lo cual se vuelve vulnerable ante posibles ataques que podría sufrir la organización. 

Finalmente, se verificó que el área de SOC no cuenta con un plan y procedimiento a seguir para la recuperación ante desastres (DR) de la herramienta SIEM. 

4.1.2.8. Informe Final de la Auditoria 

El informe final de la auditoria se llevará a cabo de forma escrita y de forma digital para ser entregado a la gerencia y se tomen las mejores decisiones, así mismo se trasferirán los documentos de trabajo donde se logró evidenciar los hallazgos que se encontraron con la finalidad de poder sustentar el informe final de la auditoria. 

 

 

 

 

24 de mayo del 2023  

Señor José Antonio Olivera 

Gerente General 

NetSecure SAC 

Av. Javier Prado Oeste 1004 

Lima, San Isidro, 15073 

Asunto: Informe Final de Auditoría  

Nos complace presentarle el informe final de auditoría correspondiente al periodo 2023-2024 de la empresa NETSECURE SAC. El objetivo general es realizar una auditoría al área de Centro de Operaciones de Seguridad (SOC), con la finalidad de evaluar si los sistemas implementados y procesos de gestión de la información cumplen con las políticas y estándares específicos de TI. 

A continuación, proporcionamos un resumen de los principales hallazgos y conclusiones derivados del proceso de auditoría: 

Resumen Ejecutivo 

En esta sección, se presenta un resumen conciso de los resultados y las recomendaciones clave obtenidas durante la auditoría. 

Se realizo una evaluación exhaustiva en el área de centro de operaciones de seguridad (SOC), se examinaron procesos, herramientas y controles a fin de garantizar la disponibilidad, integridad y confidencialidad de la organización. Se ha identificado vulnerabilidades y deficiencias en los controles y uso de herramientas y se proporcionaron recomendaciones para fortalecerlos y mitigar los riesgos potenciales. 

Alcance 

La auditoría se realizará específicamente al centro de operaciones de seguridad SOC situado en Lima, Perú ubicado en la Av. Javier Prado Oeste 1004. En las cuales se evaluarán la eficiencia y eficacia de los sistemas implementados, los procesos y procedimientos que se realizan para la gestión de eventos recepcionados. Además, se evaluará la calidad y legibilidad de los eventos registrados por la herramienta, esto se evaluará solamente la información almacenada dentro del periodo de retención definido, más no la información que están almacenadas fuera de la herramienta. Finalmente, se evaluará el plan de acción ante desastres, específicamente para las herramientas de correlación de eventos, más no de los otros sistemas del área. 

 

Tarea y funciones especificas  

Revisión de la documentación de backups. 

Revisión del manual de la herramienta SIEM. 

Revisión de plan y procedimiento de recuperación ante desastres de la herramienta SIEM. 

Revisión de políticas de seguridad implementadas en el SOC. 

Revisión del cumplimiento del SLA. 

Revisión del proceso de gestión y tratamiento de los eventos emitidos por el SIEM. 

Revisión del plan de mantenimiento de las herramientas SIEM. 

Revisión del manual de procedimiento de contingencia del SIEM. 

Revisión de los reportes semanales emitido por la herramienta SIEM para verificar si los eventos recopilados son legibles y válidos. 

Revisión de reporte del sistema operativo de la herramienta SIEM. 

 

Objetivos General y Específicos 

Objetivos General 

Realizar una auditoría al área de Centro de Operaciones de Seguridad (SOC) en la empresa NetSecure SAC, con la finalidad de evaluar si los sistemas implementados y procesos de gestión de la información cumplen con las políticas y estándares específicos de TI. 

Objetivos Especifico 

Identificar las herramientas implementadas para la gestión de eventos y la eficiencia de estos. 

Evaluar si los eventos registrados son legibles y válidos para ser procesados por la herramienta. 

Evaluar los procesos y procedimientos de la gestión de información en el SOC. 

Identificar los riesgos asociados a los sistemas implementados y brindar métodos para mitigarlo. 

Evaluar los procedimientos de contingencia de la herramienta SIEM ante una caída del principal. 

Evaluar el plan de acción de recuperación ante desastres (DR) de la herramienta SIEM. 

Evaluar si el área del SOC está cumpliendo con el SLA (acuerdo de nivel de servicio).  

Metodología: 

Ante lo presentado con anterioridad se desarrolló una metodología de tipo descriptivo-exploratorio-propositivo. Para el caso de la auditoria planteada para el área de SOC, se utilizarán los siguientes instrumentos: 

Encuestas 

La aplicación de este instrumento ha facilitado obtener información general sobre los procesos y procedimientos para la gestión de las alertas que se llevan a cabo en el área de SOC. Esta encuesta se ha realizado de manera virtual con la ayuda de herramientas a través de los formularios virtuales. 

Entrevistas 

A diferencia de la encuesta, esta herramienta ha facilitado obtener información mucho más detallado a cerca de los procesos, información del desempeño de cada herramienta administrado por el personal y los cumplimientos de las políticas corporativas.  

 

Hallazgos: 

Durante la ejecución de la auditoria a la empresa NetSecure, se encontraron diversos factores de riesgo que podrían perjudicar a la empresa en el desempeño de sus actividades. Ante esta situación, se expone las siguientes vulnerabilidades: 

Exposición de información de los clientes. 

Incumplimiento en el SLA (contrato establecido entre proveedor y cliente) por la deficiencia en la gestión de las alertas. 

Pérdidas económicas y de la reputación de la empresa. 

Pérdida y/o alteración de la información sensible. 

Eventos no recepcionados por la indisponibilidad de la herramienta. 

Eventos no procesados y recepcionados de manera correcta por la limitación de licencia de EPS. 

Gestión inadecuada de los roles de acceso en el área de operaciones. 

No hay un plan de acción específico para recuperación ante desastres (DR) de la herramienta SIEM. 

  

Recomendaciones: 

Se recomienda implementar medidas de seguridad adecuadas, como el cifrado de datos, la autenticación de usuarios y el control de acceso, para proteger la información de los clientes y evitar posibles filtraciones, apoyándose del ISO 27001. 

Se recomienda establecer procesos y sistemas de gestión de alertas eficientes, así como mecanismos de seguimiento y monitoreo para garantizar el cumplimiento de los acuerdos implantados. 

Se recomienda tomar medidas preventivas para mitigar los riesgos y contar con planes de contingencia adecuados en caso de que ocurran incidentes, se recomienda utilizar el estándar de ISO 27005 el cual trata a cerca de la gestión de riesgos de la seguridad informática. 

 

Atentamente, 

Kimberli Rosio Arias Bautista – Ing. De seguridad y auditoria informática. 

Amer Alain Talavera Urbano– Ing. De seguridad y auditoria informática. 

Helder Meléndez Guadalupe – Ing. Software. 

Jherson Estefano Leon Tito – Ing. De redes y comunicaciones. 

Semana 9 

4.1.3. Recursos 

4.1.3.1. Materiales 

Paquete de hojas bond  

Paquete de lapiceros pilot 0.5 

Paquete de Lápiz 2B 

4.1.3.2. Tecnológicos 

Cables Ethernet Rj45 Cat6 

2 computadoras Core i5 de gen10 16gb RAM, con sistema operativo Windows 11. 

4 laptops Lenovo ThinkPad i7 gen12 16gb RAM Win 11. 

1 impresora hp Smart tank 519. 

2 discos duro solido de 1TB Kingston. 

4 USB de 64GB Kingston. 

 

Software para auditoria: 

AuditBrain: Para planificar, ejecutar y documentar el trabajo según los estándares internacionales de auditoría. 

Audit Management Software: Permite desarrollar planes de auditoría específicos según el historial o a partir de indicadores de riesgo. 

TeamMate Audit: Para gestionar los diferentes aspectos relacionados con el proceso para identificar riesgos, generar informes de evaluación, programar proyectos y asignar recursos. 

ISO Tools: Para comprobar que la empresa y sus procesos se ajustan a la normativa y procedimientos ISO. 

 

4.1.3.3. Financieros 

Para el desarrollo de la Auditoria se está presentando un presupuesto, el cual es equivalente a 4 meses de trabajo. 

 

 

 

 

 

 

 

 

 4.2. Fase 2 – Ejecución del Plan de Auditoria 

4.2.1. Proceso de Recolección de Información y Planteamiento de Actividades 

Para el proceso de recolección de información se utilizó la herramienta del Formulario de Google, el cual tiene una forma práctica y sencilla de realizar encuestas de manera online, además brinda cuadros estadísticos que ayudarán a comprender la información.  

Para la recolección de información mediante las encuestas se realizarán a 15 personas del área de operaciones (monitoreo interno, Endpoint, perimetral, soporte y administración local y SOC), estas encuestas están conformadas por 15 preguntas. Asimismo, se realizarán entrevistas orientadas al personal del área de SOC para poder obtener más información y a detalle, estas entrevistas están conformadas por 6 preguntas.  

El planteamiento de la entrevista y encuesta que se presenta a continuación. 

 

4.2.2. Cuestionario Cuantitativo 

¿Selecciona a que equipos del área de operaciones perteneces? 

Monitoreo interno 

Endpoint 

Perimetral 

Soporte y administración 

SOC 

¿Cuántas veces al mes se presentó lentitud en el SIEM?  

0 - 2 

3 - 5 

6 - mas 

N.A 

¿Cuántas veces al día accede a la herramienta SIEM? 

0 - 2 

3 - 4 

5 - mas  

N.A 

¿Qué cantidad de alertas tipo falso positivo se genera al mes? 

5 - 9 

10 - 20 

20 

¿Del total de eventos procesados al mes que porcentaje se encuentra con contenido incompleto? 

0% - 3% 

3% - 5% 

5% - 10% 

¿Cuántas capacitaciones de ciberseguridad reciben al año? 

0 

1 

2 

¿Cuánto tiempo te toma en responder una alerta emitida por el SIEM? 

¿Cuántas veces al mes se envía informe a los clientes a las cuales se le brinda el servicio? 

2 min 

5 min 

10 min 

¿Cuál es el tiempo promedio de respuesta de la herramienta SIEM? 

1 min 

2 min 

3 min 

¿Cuál es el tiempo promedio que se demora para resolver un incidente de seguridad? 

10 min 

15 min 

20 min 

¿Cuántas veces al mes se envía el reporte de incidencias a los clientes? 

0 

1 

2 

¿Cuántas veces al año se realizan los backups de configuración de sistema del SIEM? 

1 

2 

3 

¿Cuántos tipos de procedimientos y gestión de eventos se manejan en el área del SOC? 

0 

1 

2 

¿Existe algún proceso que se debe seguir para la gestión de incidentes de seguridad? 

Si 

No 

¿Como calificarías el clima laboral dentro del área de SOC? 

Malo 

Bueno 

Regular 

Excelente 

¿cómo calificarías las respuestas del área de Soc. sobre las atenciones del ticket? 

Malo 

Bueno 

Regular 

Excelente 

 

 

4.2.3. Entrevistas 

¿Consideras que la herramienta SIEM cumple con los objetivos para la satisfacción de los usuarios? ¿por qué? 

_______________________________________________________________________ 

¿Consideras que los equipos brindados por la empresa son los adecuados para las tareas del día a día? ¿Por qué? 

_______________________________________________________________________ 

¿Consideras que las capacitaciones de ciberseguridad deben ser más constantes? ¿por qué? 

_______________________________________________________________________ 

¿Se cumplen las políticas y procedimientos establecidos en el área de SOC? 

_______________________________________________________________________ 

¿Qué herramientas y tecnologías se utilizan en el área de SOC? 

_______________________________________________________________________ 

¿Que otro tipo de herramientas son usadas para la gestión y tratamiento de incidencias? 

_______________________________________________________________________ 

Semana 12 

4.2.4. Técnicas y Herramientas Utilizadas 

Resumen de las herramientas como se ha utilizado 

Para el presente trabajo se utilizó dos herramientas para la recolección de información, las cuales son: Encuestas y entrevistas. En las Encuestas se trató de recolectar información relevante a la herramienta SIEM, verificar si se cumplen con los procedimientos, los tiempos de demora y las alertas generadas. Ante esta situación, esta herramienta fue utilizada con la finalidad de encontrar alguna falla durante la ejecución de sus labores. En las encuestas se ejecutaron de manera online, mediante un enlace en la cual el usuario debería marcar la respuesta que considera correcta. En el caso de las entrevistas se buscó conocer los detalles y los procedimientos de los especialistas para verificar si están correctamente informados y que siguen los protocolos establecidos por la empresa. En ejecución de la entrevista se presentaron preguntas retóricas, con la finalidad de recolectar más información y ser utilizada en la auditoria. 

4.2.5. Valoración del Riesgo 

Riesgo 

Incumplimiento del SLA (contrato establecido entre proveedor y cliente) por la deficiencia en la gestión de las alertas (6%). 

Eventos no recepcionados por la indisponibilidad de la herramienta (12%). 

Eventos no procesados y recepcionados en tiempo real de manera correcta por la limitación de licencia de EPS (20%). 

Gestión inadecuada de los roles de acceso en el área de operaciones (12%). 

Perdida de información parcial o completa por falta de un plan de acción para recuperación ante desastres (DR) de la herramienta SIEM (24%). 

Incumplimiento de políticas y procedimientos establecidos en el área de SOC para la gestión y tratamiento de las alertas (10%). 

Demora en cuanto a las atenciones de incidencias (5%). 

Exposición de información de los clientes a falta de capacitación sobre ciberseguridad al personal (28%) 

Pérdida de información por falta de definición de backup’s periódicos (8%). 

Perdida de alertas y suministro de información oportuna por la lentitud del SIEM (10%). 

 

 

Semana 13 

4.2.6. Matriz de Probabilidad e Impacto 

El Total es la suma de la puntuación generada por los riesgos e impacto referente a la tabla realizada. El resultado es un valor cuantitativo que puede ir de 0 a 100, si el valor se incrementa el impacto será aún mayor sobre los activos de la empresa.  

 

 

 

GRAVEDAD IMPACTO 

 

 

 

INSIGNIFICANTE 
 1 

BAJO 
 2 

MEDIO 
 3 

ALTO 
 4 

CATASTROFICO 
 5 

PROBABILIDAD 

FRECUENTE 

5 

  

  

  

  

  

PROBABLE 

4 

  

  

  

8 

  

OCACIONAL 

3 

  

7 

(6)(10) 

3 

  

POSIBLE 

2 

  

  

1 

(2)(4) 

5 

IMPROBABLE 

1 

  

  

  

  

9 

 

NRO DE RIESGOS 

PROBABILIDAD 

RIESGOS 

CRITERIO DE 
 EVALUACION 

VALOR DEL 
 AREA DE IMPACTO 

PUNTUACION 

1 

POSIBLE (2) 

IMCUMPLIMENTO 
 DEL SLA 

ORGANIZACIÓN 

MEDIO (3) 

6 

2 

POSIBLE (2) 

EVENTOS NO 
 RECEPCIONADOS 

SATURACION DE 
 SOFTWARE 

ALTO (4) 

8 

3 

OCACIONAL (3) 

EVENTOS NO 
 PROCESADOS 

SATURACION DE 
 SOFTWARE 

ALTO (4) 

12 

4 

POSIBLE (2) 

GESTION INADECUADA 
 DE ROLES DE ACCESO 

SEGURIDAD 
 TECNOLOGICA 

ALTO (4) 

8 

5 

POSIBLE (2) 

PERDIDA DE 
 INFORMACION 

SEGURIDAD 
 TECNOLOGICA 

CATASTROFICO (5) 

10 

6 

OCACIONAL (3) 

INCUMPLIMIENTO 
 DE POLITICAS Y PROCEDIMIENTOS 

ORGANIZACIÓN 

MEDIO (3) 

9 

7 

OCACIONAL (3) 

DEMORA FRENTE A INCIDENCIAS 

SATURACION DE 
 SOFTWARE 

BAJO (2) 

6 

8 

PROBABLE (4) 

EXPOSICION DE INFORMACIÓN 

CONFIDENCIALIDAD 

ALTO (4) 

16 

9 

IMPROBABLE (1) 

FALTA DE DEFINICION DE BACKUP´S 

SEGURIDAD 
 TECNOLOGICA 

CATASTROFICO (5) 

5 

10 

OCACIONAL (3) 

PERDIDA DE ALERTAS 

SATURACION DE 
 SOFTWARE 

MEDIO (3) 

9 

 

 

 

 

TOTAL 

89 

 

4.2.7. Herramientas de Evaluación 

Técnicas de evaluación 

INSPECCIÓN 

Se ha realizado una supervisión al proceso de gestión de incidencias de la herramienta SIEM, el cual es gestionado por el área de centro de operaciones de seguridad (SOC) tomando en consideración la documentación para este proceso, se ha verificado si los analistas realizan los procedimientos de gestión de incidencias de acuerdo con los lineamientos descritos en la documentación. Tras la aplicación de la técnica de inspección, se ha identificado que no cumplen con la totalidad de los procedimientos o algunos son omitidos. 

 

REVISIÓN DOCUMENTAL 

Con esta técnica se ha realizado las validaciones de las documentaciones y procesos internos que tiene el área de SOC, como el proceso de gestión y atención de incidencias y la documentación para solución de las incidencias. Asimismo, se realizó la inspección de los procesos que siguen los analistas en el área para la gestión de distintas incidencias que se puedan darse; además de las políticas de acceso de cada usuario a la herramienta SIEM y políticas de respaldo y recuperación de información. 

De acuerdo con el análisis y revisión de los documentos, se pudo verificar que la empresa cuenta con ciertos documentos básicos para la gestión de incidencias y alertas. Asimismo, se validó que no cumple con todos los procedimientos correctamente documentados y no hay unos documentos del debido proceso que se debe seguir para los respaldos de backups y la recuperación de estos mismo. 

COMPARACION 

De acuerdo con las revisiones realizadas de las documentaciones y manuales actuales existentes dentro del área de SOC y las documentaciones anteriores del mismo proceso, se ha podido identificar que estos documentos han sido modificados en el último año. Asimismo, se ha podido verificar que los procesos de los demás departamentos de Operaciones con respecto al área de SOC son muy diferentes; debido a que su proceso es único para la gestión de incidencias desde la herramienta SIEM. 

CONFIRMACION 

En base a las técnicas de evaluación aplicado como la inspección, revisión documental, y comparación; podemos confirmar que las documentaciones para la gestión y atención de incidencias y registros de procedimientos de las mismas; existen ya predefinidos en el área de SOC y las demás áreas del departamento Operaciones son muy diferentes para la gestión de atención de incidentes, lo cual hace que cada área tenga diferentes formas de atender y gestionar las alertas e incidencias que se pueden presentar. 

 

ACTA TESTIMONIAL 

Fecha: 20/06/23 

Oficio Número: 200-06-01 

En la ciudad de Lima siendo las 15:00 horas del día 20 de junio del 2023. Kimberli Rosio Arias Bautista, Amer Alain Talavera Urbano, Helder Meléndez y Jherson Estefano Leon Tito, ingenieros responsables de llevar a cabo la auditoria al área de centro de operaciones (SOC), hacen constatar que se llevaron a cabo la auditoria de forma legal a uno de los procesos de la empresa NetSecure ubicado en Av. Javier Prado Oeste 1004 Lima, San Isidro, 15073.  

Se levanta esta acta testimonial de auditoría a efectos de constatar los siguientes hechos encontrados. 

En la fecha y hora antes mencionadas se presentaron en el domicilio de la empresa citados anteriormente y ante la presencia del representante legal de la empresa NetSecure SAC. José Antonio Olivera, a quien se le hizo la entrega del oficio 200-06-01, mediante el cual se le hace de conocimiento sobre las pruebas fehacientes encontradas dentro de los procesos auditados en el área del SOC. Las cuales constan de las pruebas y evidencias sobre el incumplimiento de los procesos de gestión y atención de incidencias por parte de los analistas del área, quienes omiten los procedimientos previos brindados por la empresa para la correcta atención y solución de cualquier tipo de incidencias alertadas por la herramienta SIEM. 

Habiendo presentado el oficio con todas las pruebas recopiladas al señor José Antonio Olivera, quien acepta el cargo de oficio de auditoria entregado. 

 

No habiendo más hechos que constatar se da por terminado esta diligencia siendo las 18:00 horas de la misma fecha de su inicio. Asimismo, previa lectura de lo asentado los firma al margen de los fólicos presentados. Haciéndose constar que este documento fue elaborado en original y con una copia adicional. 

 

 

Fecha de entrega: 20 de junio del 2023 

 

 

 

------------------------------------------------	 

Gerente general: José Antonio Olivera		 

firma-certificado-donacion-cram - CRAMOpiniones de firma 

 

 

------------------------------------	------			--------------------------------------- 

Audit: Amer Alain Talavera				Audit: Kimberli Rosio Arias 

Manuelle Unterschrift für Dokumente auf weißem Hintergrund. Hand ...Firmas personales, Firma, Grafologia firmas 

 

-----------------------------------------			---------------------------------------- 

Audit: Helder Meléndez				Audit: Jherson Estefano Leon 

 

 

 

 

 

 

 

 

 

 

 

 

 

MATRIZ DE EVALUACION 

CRITERIOS DE EVALUACION 

EXCELENTE 

BUENO 

SUFICIENTE 

REGULAR 

DEFICIENTE 

Capacidad de detección de amenazas 

 

X 

 

 

 

Tiempo de respuesta a incidentes 

 

X 

 

 

 

Gestión eficiente de incidentes 

 

 

 

X 

 

Monitorización en tiempo real 

 

X 

 

 

 

Cumplimiento normativo 

 

 

 

X 

 

Entrenamiento y capacitación 

 

 

X 

 

 

Disponibilidad de recursos 

 

X 

 

 

 

 

 

MATRIZ FODA (DAFO) 

Fortalezas (F) 

Oportunidades (O) 

Debilidades (D) 

Amenazas (A) 

Monitoreo en tiempo real mediante uso de la herramienta SIEM 

Mayor demanda de seguridad cibernética 

Escasez de personal capacitado 

Avance tecnológico rápido 

Equipo especializado para la gestión de incidencias 

Nuevas regulaciones de seguridad 

Falta de recursos financieros 

Aumento de ataques cibernéticos 

Experiencia en gestión de incidentes 

Creciente conciencia sobre la seguridad 

Dependencia de proveedores externos 

Cambios en las regulaciones gubernamentales 

Herramientas de detección y respuesta 

Expansión del mercado a nivel Latinoamérica 

Falta de integración con otros departamentos 

Competencia en el mercado 

 

 

 

4.2.8. Hallazgos Producidos por Efecto de la Auditoria 

Hallazgo N°1 

Condición 

Se ha observado que los analistas del área de SOC no realizan los procedimientos de manera correcta para la atención de alertas, ya que algunos de los procedimientos son omitidos, lo cual hace que exista una deficiencia en la atención oportuna de las mismas. 

Criterio 

Lo cual contraviene a los protocolos y políticas establecidas por la empresa, ya que, según las políticas internas definidas, se deben seguir los procedimientos para la atención de tickets. 

Causa 

La causa principal de la omisión de procedimientos podría deberse a falta de conocimiento y capacitación al personal sobre el uso de estos. 

Efecto 

Las consecuencias que podría traer este caso es la mala gestión y atención de las alertas, e incluso la atención inadecuada de las mismas el cual podría causar algún impacto negativo en sus clientes. 

Recomendación 

Se recomienda brindar una orientación y capacitación adecuada a los analistas sobre el uso de los procedimientos para la atención de alertas. 

Conclusiones 

Es importante que se cumpla con los procedimientos para la gestión y atención de las alertas, ya que esto podría favoreces a la organización, para dar una atención de manera correcta y oportuna de las mismas. 

Hallazgo N°2 

Condición 

Se ha identificado que la herramienta SIEM no recepciona todos los eventos de manera correcta. 

Criterio 

Lo cual contraviene al Acuerdo de Nivel Operacional (OLA) y al ISO/IEC 20000, el cual define que cuyo propósito es cumplir con los requisitos de gestión de nivel de servicio. 

Causa 

La causa principal de es debido a la capacidad de procesamiento de la herramienta es muy limitada y por la limitación de la licencia de recepción de eventos por segundo EPS. 

Efecto 

La consecuencia que podría traer este caso, que el incumplimiento del contrato a nivel Operacional (OLA) y esto podría llegar a problemas mayores. 

Recomendación 

Se recomienda prestar especial atención a este caso, para resolver el problema con la lentitud de la herramienta y ampliar la capacidad de licencia de eventos por segundo (EPS). 

Conclusiones 

Es muy importante que la herramienta SIEM, esté siempre operativo para recepecionar y correlacionar los eventos de manera correcta. 

Hallazgo N°3 
Condición 

Tras las revisiones de los reportes de la herramienta SIEM se ha identificado que existen eventos no procesados y correlacionados de manera correcta, ya que existen datos y campos vacíos en los eventos; esto podría deberse a la limitación de la licencia EPS 

Criterio 

El criterio utilizado es la capacidad limitada de la licencia EPS, que restringe el número de eventos que pueden ser procesados y correlacionados correctamente. 

Causa 

La causa principal de este problema es la limitación de la licencia EPS, que impide el procesamiento adecuado de todos los eventos registrados debido a su cantidad limitada. 

Efecto 

El efecto de esta limitación es que algunos eventos no son procesados y correlacionados correctamente, lo que puede llevar a la falta de detección de amenazas y vulnerabilidades importantes en el entorno de seguridad. 

Recomendación 

Para abordar este problema, se recomienda considerar una actualización de la licencia EPS para aumentar su capacidad y permitir el procesamiento adecuado de todos los eventos. Esto garantizará una mayor eficacia en la detección de amenazas y una mejor correlación de eventos en la herramienta SIEM. 

Conclusión 

La limitación de la licencia EPS está causando eventos no procesados y correlacionados de manera incorrecta en la herramienta SIEM. Para solucionar este problema, se recomienda actualizar la licencia para aumentar su capacidad y garantizar un mejor funcionamiento del sistema de seguridad. 

Hallazgo N°4 

Condición 

Se ha observado que existe roles de acceso no definidos a la herramienta SIEM, ya que 	algunos usuarios que cuentan con este acceso no son analistas del SOC y que tienen 	permisos de acceso tipo administrador sobre la herramienta.  

Criterio 

Se debería tener en cuenta el marco NISP SP 800-53, el cual ofrece pautas y mejoras prácticas en la materia de seguridad y la gestión de acceso. De esta manera, se tendría una mejor gestión de los accesos de los analistas y los administradores para ingresar a la herramienta SIEM. 

Causa 

Alguna de las causas posibles que existiría serían las siguientes: falta de planificación, cambios en los roles de los usuarios, deficiencia en los procesos de gestión de acceso, falta de conciencia sobre los riesgos de seguridad. 

Efecto 

De las causas definidas anteriormente se puede concluir que existirían riesgos ante el acceso de un usuario no apto para el manejo de la herramienta, asimismo se podrían vulnerar datos. 

Recomendación 

Se recomienda que los accesos sean definidos con cautela y que se encuentre organizado, de esta manera cada usuario tendría el acceso correcto y que este autorizado por los administradores para realizar algún cambio en la herramienta 

Conclusiones 

Considero que los hallazgos son importantes ya que es una manera practica de poder identificar problemas existentes ante una mala gestión del control de acceso de los usuarios y administradores, lo cual podría generar problemas y adversidades en el funcionamiento de la herramienta 

Hallazgo N°5 

Condición 

Tras las revisiones realizadas de los procedimientos y las documentaciones del plan de acción de recuperación ante desastres (DR) de la herramienta SIEM, se ha verificado que el plan de acción con lo que se cuenta el SOC no está actualizado. 

Criterio 

Según la norma ISO 27001 establecer un adecuado plan de contingencia minimiza las pérdidas en caso de desastre y facilita la reanudación de las operaciones de una forma rápida, eficaz y oportuna. 

Causa 

Las causas probables que pueden ocurrir ante las revisiones de los procedimientos y documentación de plan de acción de recuperación ante un desastre pueden ser: la identificación de deficiencia y errores, la experiencia de incidentes previos, cambios de entorno o riesgos que pueden presentarse en un futuro. 

Efecto 

Los efectos que se pueden producir son la ineficacia en la respuesta ante los desastres, la falta de oportunidades de identificar posibles brechas en el plan de acción de recuperación, la desactualización de información, la falta de cumplimiento normativo y la deficiencia de aprendizaje y mejora continua. 

Recomendación 

Se recomienda que la revisión de los procedimientos y las documentaciones del plan de acción de recuperación de desastres estén actualizados constantemente y que se apliquen todas las modificaciones, con el fin de prevenir fallos ante algún incidente ocurrido. 

Conclusiones 

En conclusión, se puede apreciar que la falta de actualización en la documentación del plan de acción puede ser riesgoso para la herramienta, ya que los usuarios no estarían informados de todos los procedimientos que se debe seguir si ocurre algún incidente 

Hallazgo N°6 

Condición 

Según el análisis realizado de las métricas y el tiempo de atención de las incidencias, se detectó que existe una demora de más de 20 minutos para la resolución de una incidencia de menor grado. 

Criterio 

Se visualiza a la norma ISO/IEC27035:2016 la cual aborda aspectos relacionados con las métricas y el tiempo de atención de las incidencias. 

Causa 

Las causas probables que puede existir ante una demora en la resolución de una incidencia de menor grado son: la falta de asignación adecuada de recursos, los procesos de escalado son ineficientes, no existe una priorización adecuada, deficiencia en la documentación y problemas de comunicación interna. 

Efecto 

Los efectos producidos podrían ser: impacto en la productividad, frustración y descontento de los usuarios, riesgo de escalada de la incidencia, deterioro de la seguridad, pérdida de visibilidad y control, aumento d tiempo de recuperación, entre otros. 

Recomendación 

Se recomendaría tomar acciones en evaluar y confirmar la prioridad del incidente, comunicarse con el equipo de respuesta de incidencia, realizar un seguimiento proactivo, analizar y mejorar los procesos 

Conclusiones 

En conclusión, la demora de 20 puede afectar significativamente a la empresa, ya que podría obstruir las actividades que se realizan de manera rutinaria. 

Hallazgo N°7 

Condición 

Se ha revisado el proceso y la documentación de backup que se realizan a la herramienta SIEM, donde se identificó que no está bien definido los tipos de backup que se realiza (backup de sistema y backup de la información) y la frecuencia de la realización de estas. 

Criterio 

El criterio utilizado es la falta de una definición clara de los tipos de backup y la falta de una frecuencia adecuada para realizarlos. 

Causa 

La causa principal de esta situación es la falta de una política o procedimiento establecido que defina claramente los tipos de backup necesarios para la herramienta SIEM y la frecuencia con la que deben realizarse. 

Efecto 

El efecto de esta falta de definición y frecuencia inadecuada de los backups es un mayor riesgo de pérdida de datos y de la incapacidad para restaurar la herramienta SIEM en caso de fallos o incidentes. 

Recomendación 

Para abordar este problema, se recomienda desarrollar una política de backup clara y establecer los tipos de backup (backup de sistema y backup de información) necesarios para la herramienta SIEM. Además, se debe definir una frecuencia adecuada para realizar los backups y documentar estos procesos correctamente. 

Conclusión 

La falta de definición de los tipos de backup y la frecuencia inadecuada de realización de estos en la herramienta SIEM representan un riesgo para la pérdida de datos y la incapacidad de restaurar la herramienta en caso de fallos. Es necesario establecer una política de backup clara, definir los tipos de backup necesarios y establecer una frecuencia adecuada para realizarlos, además de documentar adecuadamente estos procesos. 

Hallazgo N°8 
Condición 

Después de analizar los reportes de las alertas emitidas por la herramienta SIEM, se ha identificado que aproximadamente de 10 a 20 alertas al mes son falsos positivos, es decir, alertas que indican la existencia de una amenaza o incidente que en realidad no es real. 

Criterio 

El criterio utilizado es el número significativo de alertas falsas positivas que se generan en un periodo de un mes. 

Causa 

La causa principal de este problema puede ser la falta de una configuración precisa de las reglas y los umbrales de detección de la herramienta SIEM, lo que lleva a la generación de alertas incorrectas. 

Efecto 

El efecto de estas alertas falsas positivas es la generación de ruido y distracción para el equipo de seguridad, lo que puede afectar la eficiencia y la capacidad de respuesta a amenazas reales. Además, puede generar una falta de confianza en las alertas emitidas por la herramienta SIEM. 

Recomendación 

Para abordar este problema, se recomienda revisar y ajustar la configuración de las reglas y los umbrales de detección de la herramienta SIEM. Esto implica un análisis más exhaustivo de los patrones de comportamiento y la personalización de las reglas de detección para reducir la cantidad de alertas falsas positivas. Además, se sugiere implementar mecanismos de retroalimentación y revisión continua para mejorar la precisión de las alertas y reducir aún más los falsos positivos. 

Conclusión 

La presencia de 10 a 20 alertas falsas positivas al mes en la herramienta SIEM puede afectar negativamente la eficiencia y la capacidad de respuesta del equipo de seguridad. Se recomienda ajustar la configuración de las reglas y los umbrales de detección, así como implementar mecanismos de retroalimentación y revisión continua para reducir la cantidad de alertas falsas positivas y mejorar la confiabilidad de las alertas emitidas por la herramienta SIEM. 

Hallazgo N°9 

Condición 

Se ha observado que existe deficiencia en las capacitaciones que se les brinda al personal de las áreas de operaciones y SOC sobre ciberseguridad. 

Criterio 

El criterio utilizado es la falta de capacitación adecuada y actualizada en ciberseguridad para el personal de estas áreas. 

Causa 

La causa principal de esta deficiencia puede ser la falta de recursos o planificación insuficiente para proporcionar capacitaciones adecuadas sobre ciberseguridad al personal de operaciones y SOC. También puede deberse a la falta de conocimiento o experiencia en el diseño y la implementación de programas de capacitación en ciberseguridad. 

Efecto 

El efecto de esta deficiencia en las capacitaciones es una menor preparación del personal para enfrentar y responder a amenazas e incidentes de ciberseguridad. Esto puede resultar en una mayor vulnerabilidad de la infraestructura y los datos de la organización, así como en una respuesta ineficiente a posibles incidentes. 

Recomendación 

Para abordar esta situación, se recomienda desarrollar e implementar programas de capacitación en ciberseguridad específicamente diseñados para el personal de operaciones y SOC. Estas capacitaciones deben ser periódicas, actualizadas y adaptadas a las necesidades y roles específicos de los empleados. Además, se sugiere la contratación de profesionales o consultores especializados en ciberseguridad para brindar capacitación y orientación adecuada. 

Conclusión 

La deficiencia en las capacitaciones brindadas al personal de operaciones y SOC en ciberseguridad representa un riesgo para la organización, ya que puede resultar en una menor preparación y respuesta ineficiente ante amenazas e incidentes de seguridad. Es esencial desarrollar programas de capacitación adecuados, actualizados y adaptados a las necesidades del personal, y considerar la contratación de expertos en ciberseguridad para mejorar la calidad de la capacitación y fortalecer las habilidades del personal en esta área crítica. 

 

 

 

Semana 14 

  

4.3. Fase 8 – Informe de la Auditoria 

4.3.1. Introducción al Informe 

Junio de 2023 

Auditor responsable: Kimberli Arias Bautista 

El presente informe tiene la finalidad de proporcionar una visión general del cumplimiento y la existencia de los procesos y procedimientos internos del área del SOC.  

Asimismo, tiene como objetivo brindar con mayor detalle de los hallazgos obtenidos durante la auditoria, cada hallazgo se ha clasificado según su gravedad en un matriz de riesgos y se ha proporcionado una descripción detallada, junto con las implicaciones asociadas y las recomendaciones correspondientes para mejorar los controles y mitigar los riesgos identificados. Es importante destacar que este informe representa una instantánea de la situación en el momento de la auditoría, basada en los datos y la información disponibles del periodo marzo 2023 hasta el presente mes Junio. Por lo tanto, algunas circunstancias o eventos posteriores pueden haber ocurrido y no se reflejarán en este informe. 

A continuación, se presentan los puntos más importantes que se han desarrollado durante la auditoria en la empresa NetSecure SAC  

El objetivo general de esta auditoría fue auditar al proceso interno del área de Centro de Operaciones de Seguridad (SOC) en la empresa NetSecure SAC, con la finalidad de evaluar si los sistemas implementados y procesos de gestión de la información cumplen con las políticas y estándares específicos de TI. El alcance de la auditoria fue específicamente al centro de operaciones de seguridad SOC situado en Lima, Perú. En las cuales se evaluaron la eficiencia y eficacia de los sistemas implementados, los procesos y procedimientos que se realizan para la gestión de eventos recepcionados. 

Las metodologías que han sido usadas para obtener información de los procesos fueron entrevistas y encuestas, con estas metodologías se han obtenido información sobre los procesos y procedimientos que se manejan dentro del área, asimismo, se ha obtenido algunas posibles vulnerabilidades, amenazas y riegos que pueden causar algún impacto en la seguridad de la información de la organización y de sus clientes. A continuación, se presenta las principales observaciones. 

4.3.2. Principales Observaciones 

 Algunas principales observaciones que se ha detectado al momento de realizar la auditoria se centran en los hallazgos obtenidos, de los cuales se pasará a detallarlos de manera específica. 

Los hallazgos que presentan un mayor porcentaje de observaciones son los siguientes: 

Analistas del área de SOC no realizan los procedimientos de manera correcta para la atención de alertas. Se eligió este hallazgo porque presenta problemas en la mala gestión y en la atención de alertas, ya que ocasionaría problemas con un impacto negativo hacían los clientes. 

 
Se presentan eventos no procesados y correlacionados de manera correcta, puesto que, al existir datos y campos vacíos en los eventos ocasionarían riesgos de monitoreo y falta de información, este hallazgo se debe a la limitación de la licencia de EPS 

Existen roles de acceso no definidos a la herramienta SIEM, este es un problema de alto riesgo, porque al no existir un rol definido podrían modificar cambios en la herramienta, generando inconvenientes al momento de emitir lo eventos y recaudar la información 

Se ha revisado el proceso y la documentación de backup que se realizan a la herramienta SIEM, donde se identificó que no está bien definido los tipos de backup que se realiza (backup de sistema y backup de la información) y la frecuencia de la realización de estas, porque al momento de presentar algún incidente no se tendría la certeza de verificar si la información entrega es correcta o se tardaría más tiempo en detectar cual es el problema que se ha presentado. 

Se ha observado que existe deficiencia en las capacitaciones que se les brinda al personal de las áreas de operaciones y SOC sobre ciberseguridad, porque al no existir una capacitación permanente las personas encargadas de solucionar los errores presentarán mayor dificultad de solventarlas.	 

 

Semana 15-Entrega de Avance de Proyecto Auditoria 

  

4.3.3. Recomendaciones y Plan de Acción / Mejoras 

  

Semana 16 Exposición final de proyecto por grupos 

Semana 17 Exposición final de proyecto por grupos 

Semana 18 Entrega de Trabajo Final en Canvas 

 

Anexo 

Identificar Activos: 

Infraestructura Física 

Licencias de software 

Equipos móviles 

Endpoints 

Personal 

USB 

Servidores 

Backup 

Información digital y física 

Matriz de Riego: 

Tabla, Escala de tiempo

Descripción generada automáticamente 

6 responsabilidades que asumiremos como auditores: 

Evaluar la información de la organización (Integridad, Confidencialidad, Disponibilidad y Completitud) 

Evaluar si los recursos tecnológicos se utilizan en forma eficiente y en 
concordancia con los requerimientos del negocio. 

Evaluar los planes de recuperación de desastres y recuperación de negocio. 

Verificar que se cumplan con las políticas corporativas y con las regulaciones y normas. 

Evaluar la seguridad física y lógica de los activos TI. 

Evaluar los riesgos de los sistemas de información. 

 

 

5 ventajas del uso de las tecnologías de la información 

 

Desarrollo de nuevas habilidades del personal 

Capacitaciones personalizadas a los trabajadores 

Automatización de procesos usando las herramientas para la gestión de la información. 

Aumento de productividad 

Facilita el acceso a la información 

 

5 desventajas del uso de las tecnologías de la información 

Dependencia en el uso de la tecnología y/o procesos 

Disminuye la interacción de los trabajadores 

Amenaza a la seguridad de la información 

Reducción de la creatividad 

 

2 controles aplicados a las tecnologías de la información 

Controles de preinstalación: Este control se aplicaría en el caso de una instalación o implementación de una tecnología nueva, ya que se requiere validar las ventajas, características y compatibilidad de esta con las otras herramientas ya existentes. Asimismo, se debe evaluar la viabilidad de la capacitación al personal para la gestión de esta nueva tecnología. 

Control de la documentación: Este control se debe aplicar en la organización para que   todo sus procesos y procedimientos estén correctamente documentados y actualizados. Asimismo, estas documentaciones y el historial de cambios realizados deben estar respaldadas. 

4 controles internos aplicados al proyecto 

Control de explotación de sistemas de información. 

Para el caso del proyecto, este control aplica a nivel de gestión de planificación, adquisición y de requerimientos de hardware para la implementación de soluciones de seguridad TI. 

Control en aplicaciones  

Aplica a nivel de gestión de actualización de aplicaciones de las herramientas de seguridad TI 

Control informático sobre redes 

Aplica para la gestión de mantenimiento preventivo de las herramientas y soluciones de seguridad TI. 

Controles sobre computadores y redes de área local. 

Control para las políticas de adquisición de nuevos equipos, servidores para la organización. 

 

Preguntas de Entrevistas: 

1. ¿Consideras que la herramienta SIEM cumple con los objetivos para la satisfacción de los usuarios? ¿por qué? 4 respuestas 

Sí, porque la herramienta SIEM analiza datos de gran cantidad y genera un reporte, el cual nos ayudará a verificar si toda la información es correcta 

Si, ya que es una herramienta muy versátil que nos permite visualizar los eventos en tiempo real y permite generar reportes para temas de auditoría del cliente. 

Si, ya que permite alertar a los clientes mediante una serie de procesos con la finalidad de prevenir posibles ataques cibernéticos a los usuarios finales. 

sí, porque todos los reportes enviados de manera semanal incluyen todos los datos necesarios para que el cliente pueda realizar el seguimiento necesario. 

 

2. ¿Consideras que los equipos brindados por la empresa son los adecuados para las tareas del día a día? ¿Por qué?  
4 respuestas 

Sí, porque cumple con las expectativas y con las especificaciones de los programas para tener un trabajo adecuado. 

Si, la empresa proporciona equipos que tienen mayor capacidad para poder desarrollar las tareas del día a día. 

Si, ya que son equipos con buenas características que están por encima de Core i7 10ma generación y 16 de RAM. 

sí, porque permite ejecutar las herramientas necesarias para realizar las tareas de manera optimo. 

 

3. ¿Consideras que las capacitaciones de ciberseguridad deben ser más constantes? ¿por qué? 4 respuestas 

Sí, porque de esa manera estaremos más alertas a los ataques que se estén presentando y poder solucionar de manera rápida. 

Si, la empresa nos brinda capacitaciones con poca frecuencia con respecto a temas de ciberseguridad, estas capacitaciones frecuentes podrían ayudarnos a tener más conciencia y reducir cualquier riesgo de seguridad. 

Si, ya que cada día crean nuevas formas de vulnerar los sistemas y tener capacitaciones más constantes podrían ayudaría a la empresa a tener una mejor seguridad a nivel informático. 

sí, con la evolución constante de la tecnología, surgen nuevas amenazas y técnicas de ataques, por lo tanto, es importante recibir capacitaciones para poder estar al tanto a cerca de las últimas medidas de seguridad que se debe implementar en una organización. 

 

4. ¿Se cumplen las políticas y procedimientos establecidos en el área de SOC?  
4 respuestas 

Si, porque con las políticas y los procedimientos nos servirán para guiarnos y utilizar bien las herramientas que se tiene en el área. 

Si, existen ciertos procedimientos que se debe seguir en el área de SOC, como por ejemplo para la atención y gestión de incidencias. Asimismo, existen políticas internas que se debe seguir para el caso de escalamiento de ticket con los especialistas. 

Si se cumplen, ya que existen manuales para los procedimientos de cada tarea, lo cual permiten procedimientos bien gestionados. 

si se cumplen, ya que es importante cumplir las políticas cuando uno gestiona incidencias de seguridad y los procedimientos se deben respetar para que dicha incidencia pueda ser tratada de manera adecuada. 

 

5. ¿Qué herramientas y tecnologías se utilizan en el área de SOC?  
4 respuestas 

SIEM, UEBA, EDR 

Se usa principalmente la herramienta SIEM para el monitoreo de seguridad de los dispositivos, Nagios para el monitoreo de disponibilidad de los dispositivos, SOAR para la generación y gestión de alertas que son emitidas por el SIEM y OTRS para el registro y seguimiento de ticket. 

Se utilizan las herramientas de monitoreo y gestión de eventos como SIEM y para la detección y respuesta de endpoint EDR que ayuda a investigar amenazas dirigidas a puntos finales o hosts. 

se utiliza diferentes herramientas como el SOAR, IDS/IPS, NAGIOS Y SIEM. el SIEM sirve para la recopilación y centralización de datos proveniente de otros sistemas. 

 

6. ¿Qué otro tipo de herramientas son usadas para la gestión y tratamiento de incidencias?  
4 respuestas 

JIRA, utilizaría esta herramienta porque gestiona incidentes, hace seguimientos y análisis 

Para la gestión de incidencias se usa el SIEM, ya que nos ayuda a tener una visibilidad amplia y a detalle del incidente ocurrido, de esa manera podemos realizar el seguimiento correspondiente y poder detectar a tiempo cualquier tipo de incidencias de seguridad. 

SOAR el cual permite recopilar entradas monitoreadas así mismo se utiliza el SIEM que mediante de un análisis busca de un comportamiento anómalo y NAGIOS que sirve para vigilar equipos y servicios, enviando una alerta cuando el comportamiento de los mismos no sea el deseado. 

Plataformas de gestión de incidentes, Herramientas de colaboración y comunicación, Sistemas de gestión de configuraciones, entre otros. 

 

Preguntas de Encuestas: 

Gráfico de las respuestas de Formularios. Título de la pregunta: 1. ¿Selecciona a que equipo del área de operaciones perteneces? 
. Número de respuestas: 16 respuestas. 

Gráfico de las respuestas de Formularios. Título de la pregunta: 2. ¿Cuántas veces al mes se presentó lentitud en el SIEM?    . Número de respuestas: 16 respuestas. 

Gráfico de las respuestas de Formularios. Título de la pregunta: 3. ¿Cuántas veces al día accede a la herramienta SIEM? 
. Número de respuestas: 16 respuestas. 

Gráfico de las respuestas de Formularios. Título de la pregunta: 4. ¿Qué cantidad de alertas tipo falso positivo se genera al mes? 
. Número de respuestas: 16 respuestas. 

Gráfico de las respuestas de Formularios. Título de la pregunta: 5. ¿Del total de eventos procesados al mes que porcentaje se encuentra con contenido incompleto? 
. Número de respuestas: 16 respuestas. 

Gráfico de las respuestas de Formularios. Título de la pregunta: 6. ¿Cuántas capacitaciones de ciberseguridad reciben al año? 
. Número de respuestas: 16 respuestas. 

Gráfico de las respuestas de Formularios. Título de la pregunta: 7. ¿Cuánto tiempo te toma en responder una alerta emitida por el SIEM? 
. Número de respuestas: 16 respuestas. 

Gráfico de las respuestas de Formularios. Título de la pregunta: 8. ¿Cuál es el tiempo promedio de respuesta de la herramienta SIEM? 
. Número de respuestas: 16 respuestas. 

Gráfico de las respuestas de Formularios. Título de la pregunta: 9. ¿Cuál es el tiempo promedio que se demora para resolver un incidente de seguridad? . Número de respuestas: 16 respuestas. 

Gráfico de las respuestas de Formularios. Título de la pregunta: 10. ¿Cuántas veces al mes se envía el reporte de incidencias a los clientes? 
. Número de respuestas: 16 respuestas. 

Gráfico de las respuestas de Formularios. Título de la pregunta: 11. ¿Cuántas veces al año se realizan los backups de configuración de sistema del SIEM? 
. Número de respuestas: 16 respuestas. 

Gráfico de las respuestas de Formularios. Título de la pregunta: 12.  ¿Cuántos tipos de procedimientos y gestión de eventos se manejan en el área del SOC? . Número de respuestas: 16 respuestas. 

Gráfico de las respuestas de Formularios. Título de la pregunta: 13. ¿Existe algún proceso que se debe seguir para la gestión de incidentes de seguridad? 
. Número de respuestas: 16 respuestas. 

Gráfico de las respuestas de Formularios. Título de la pregunta: 14. ¿Cómo calificarías el clima laboral dentro del área de operaciones? 
. Número de respuestas: 16 respuestas. 

Gráfico de las respuestas de Formularios. Título de la pregunta: 15 ¿Cómo calificarías las respuestas del área de operaciones, sobre los tickets asignados por soporte y administración? 
. Número de respuestas: 16 respuestas. 

 

 

Incumplimiento de los SLA 

Condición 

De acuerdo a la revisión de los términos de contratos de servicios entre las dos partes, se ha evidenciado que estos acuerdos no se están cumpliendo según lo esperado. 

Criterio 

Esto contraviene a la guía de buenas prácticas de ITIL el cual sirve para la gestión de servicios de TI ampliamente utilizada. Proporciona un marco para la gestión de servicios de TI, incluyendo la gestión de niveles de servicio y la elaboración de SLA. 

Causa 

Alguna de las causas que se han encontrado es por la falta de capacidad para el cumplimiento de los niveles de servicios acordado, existen problemas de lentitud y saturación con las herramientas de procesamiento de eventos y la deficiencia en la gestión de los incidentes y alertas. 

Efecto 

La consecuencia que traería para la empresa sería como la pérdida de confianza y credibilidad de los clientes, impacto en la reputación de la empresa y hasta podría tener demandas por parte de los clientes. 

Recomendación. 

Se recomienda tener en consideración la definición de los objetivos y las métricas, la comunicación efectiva con el cliente y sobre todo el monitoreo constante de los cumplimientos de los SLA 

Conclusiones 

El cumplimiento del SLA es fundamental para establecer y poder mantener una relación sólida entre el proveedor y el cliente, por lo tanto, debe haber confianza y satisfacción del cliente, mejorar la calidad de servicio y la maximización del servicio. Todo ello al priorizar el cumplimiento de los SLA, las organizaciones pueden fomentar relaciones sólidas y satisfactorias con sus clientes y obtener ventajas competitivas en el mercado. 

Eventos no recepcionados por la indisponibilidad de la herramienta 

Condición 

Se ha identificado que la herramienta no recepciona todos los eventos, esto sucede porque la capacidad de procesamiento de la herramienta es muy limitada y hace que deje de trabajar por un tiempo y ello genera pérdida de eventos los cuales son reportados por las distintas herramientas hacia el SIEM 

Criterio 

Este escenario no cumple con los estándares que indica el ISO 27001 el cual indica que es muy importante la adecuada gestión de las incidencias de la seguridad de la información el cual va de la mano con el SGSI. 

Causa 

La principal causa para que esto ocurra ha sido por la falta capacidad de procesamiento de la herramienta SIEM ya que la parte de hardware es muy limitada, por ello es que se satura la herramienta. 

Efecto 

Teniendo identificado la causa, se puede determinar las consecuencias que podrían afectar a la empresa al cual se le presta el servicio, por ejemplo, si en ese evento no recepcionado podría haber algún tipo de intrusión maligno y no se haya identificado la incidencia, traería consecuencias fatales para la empresa, se puede hablar de pérdidas de información sensible y pérdidas de prestigio de la empresa que brinda el servicio de seguridad. 

recomendación 

Se recomienda a la alta gerencia realizar una adecuada recopilación de información acerca de las características de la herramienta y poder mejorar el tema del hardware para el adecuado procesamiento de los datos, tomando siempre los niveles de procesamiento óptimo para el adecuado funcionamiento. 

Conclusión 

Es importante el funcionamiento correcto de las herramientas, más aún si se trata de la seguridad de la información, por lo tanto, si no existe un funcionamiento óptimo de las herramientas, todos los procesos relacionados no trabajaran adecuadamente. En ese sentido los auditores entregan el informe con las recomendaciones con el fin de que la alta gerencia pueda tomar o no las decisiones de realizar las mejoras. 

Eventos no procesados y recepcionados de manera correcta 

Condición 

Según la ejecución de la Herramienta SIEM se detectó que los eventos emitidos no podrían ser procesados y recepcionados de manera correcta, ya que existiría errores en la configuración, sobre carga de eventos y falta de datos. 

Criterio 

No existe una norma previamente hecha para los eventos no procesados y recepcionados. Sin embargo, la norma ISO 27001 promueve la necesidad de identificar, analizar y evaluar los eventos de manera adecuada. 

Causa 

Algunas causas posibles que podría ocurrir a partir de los eventos no procesador y recepcionados de manera correcta serían los siguientes: configuración incorrecta, falta de integración de datos, recursos insuficientes, sobre carga de eventos, entre otros. 

Efecto 

La Herramienta SIEM pueden resultar en una menor capacidad para detectar y responder a amenazas de seguridad, una pérdida de visibilidad y contexto, un rendimiento ineficiente y dificultades en la gestión operativa.  

Recomendación 

Es fundamental abordar estas cuestiones mediante una revisión y ajuste adecuado de la configuración, la integración de datos y la asignación de recursos necesarios para garantizar un funcionamiento óptimo del SIEM. 

Conclusiones 

Considero que los hallazgos son importantes ya que es una manera práctica de poder identificar un defecto que tendría la herramienta en la empresa, asimismo buscar soluciones de manera eficaz y rápida con la finalidad de solventar los errores y mejorar la recepción de los eventos en el SIEM. 

Incumplimiento con los procesos internos para la gestión de incidencias 

Condición 

Según el análisis realizado, se detectó que algunos analistas que trabajan en el área de SOC no cumplen con los pasos y procesos adecuados a seguir frente a una incidencia, a pesar de que existe un manual de procedimientos a seguir. 

Criterio 

Frente a esta situación se infringe la norma de ITILv3 mejores prácticas referentes a la gestión de servicios TI en el cual se describe detalladamente un extenso conjunto de funciones y procesos ideados para ayudar a las organizaciones a lograr calidad y eficiencia en las operaciones de TI. 

Causa 

Malas prácticas por parte del personal del área de SOC o falta de capacitaciones. 

Efecto 

La consecuencia que traería el incumplimiento de los procesos internos es que pueda dar una mala gestión y tratamiento de un incidente de mayor grado, lo cual puede decantar en el incumplimiento de los contratos a nivel de servicio con los clientes (SLA) e incluso puede darse  la no resolución correcta de un incidente que pueda afectar a la organización. 

Recomendación 

Se recomienda brindar capacitaciones constantes para el cumplimiento de los procesos y supervisar al personal del área de SOC de que se esté cumpliendo los procesos establecidos.  

Conclusiones 

Considero que los hallazgos son importantes, ya que nos ayudan a descubrir los defectos que presentan las empresas, en el que se indica condición, criterio causa y efecto. Además, que permite realizar acciones correctivas en un tiempo justo para no generar incidencias, siempre y cuando la empresa emita una opinión asertiva frente a la auditoría realizada y acepte las recomendaciones 

Diagrama de caso de uso 

 

 
