Si bien el proceso de gestión de incidentes es adaptable para responder a ataques tipo Advanced Persistence Threat (APT), y se deben tomar ciertas medidas para cualquier incidente, independientemente de la amenaza, existen estrategias de respuesta más adecuadas para una amenaza de tipo APT. Esta lista busca proponer acciones apropiadas para abordar este tipo de amenaza puntual. Siempre será recomendada una adaptación personalizada a cada entorno y situación. Sin embargo, esta guía ofrece un conjunto general de acciones apropiadas para la respuesta a una amenaza APT.

# Preparación

- [ ] Identificar la propiedad y la responsabilidad de todos los sistemas (incluidos los datos) de la empresa.
- [ ] Canales de comunicación claros.
  - [ ] Capacidades para la comunicación por correo electrónico cifrado (posiblemente sin utilizar el servidor de correo electrónico principal).
  - [ ] Capacidades de mensajería de chat cifrado (posiblemente sin poder hacer uso del servidor de chat principal).
  - [ ] Lista de llamadas telefónicas para la coordinación, almacenada en recursos sin conexión a Internet.
  - [ ] Definición de lista de notificación.
    - [ ] Documentar una lista de contactos por sistema.
      - [ ] Propietario del sistema.
          - [ ] Definición del Punto de Contacto (POC).
      - [ ] POC técnicos.
        - [ ] Posibilidad de contacto fuera del horario laboral / rotación / lista de números para obtener una respuesta.
- [ ] Respuesta a incidentes con capacidades de abordar ataques de tipo APT.
  - [ ] Comprensión clara de las características de esta amenaza.
    - [ ] Comprensión de la gerencia de manera clara de este tipo de amenaza.
  - [ ] Autorización escrita para autorización de respuesta requerida en todos los sistemas de la empresa.
    - [ ] Recursos para realizar investigaciones extensas.
        - [ ] Si la gestión de incidentes actualmente no es 24/7, ¿qué recursos están disponibles para continuar con el trabajo de IR durante la respuesta continua?
- [ ] Capacidad interna o de terceros con capacidades para.
  - [ ] Respuesta a incidentes.
  - [ ] Investigación forense digital.
  - [ ] Ingeniería inversa de malware
- [ ] Documentación de estrategia de contención para APT
  - [ ] Documentación y preparación en estrategias básicas:
    - [ ] Observar y aprender
    - [ ] Desconectar
  - [ ] Definir los procedimientos operativos estándar (POE) para cada escenario
  - [ ] Definir una metodología para que el equipo de respuesta a incidentes se desvíe de los POE según sea necesario
    - [ ] Esta metodología debe formar parte de los POE
      - [ ] Incluir los pasos para la notificación y justificación de las desviaciones planificadas
- [ ] Establecimiento del Equipo de prensa asociado a respuesta a incidentes
- [ ] Establecimiento del Equipo legal asociado a respuesta a incidentes

# Identificación

- [ ] Remote Access Trojan (RAT)
- [ ] Comando y control (C2)
- [ ] Descubrimiento de comunicaciones cifradas
- [ ] Descubrimiento de canal encubierto 
- [ ] Alertamiento de IDS/IPS basado en host, EDR o XDR sobre llamadas inesperadas al sistema, acceso a datos, puerto abierto
- [ ] Notificación externa directa (Fuerzas policiales, socios comerciales)
- [ ] Notificación externa indirecta (Tareas de Inteligencia de Ameanzas sobre comportamientos anómalos, búsqueda dentro del entorno)
- [ ] Identificación de Datos fuera de la organización (pastebin, foros, deep y dark web)
- [ ] Comunicaciones generadas por agentes de amanza 
- [ ] La notificación al personal interno debe realizarse de forma discreta y segura.
  - [ ] Cifrada
  - [ ] Limitada solo a quienes necesitan saberlo
  - [ ] La autorización para agregar recursos adicionales a la respuesta a incidentes se limita al equipo de Gestión de Respuesta a Incidentes o a la Gestión de la Unidad de Negocio.
  - [ ]Categorizar la gravedad y el impacto conocidos
  - [ ] Proporcionar actualizaciones a medida que se revele nueva información importante
     
# Contención

- [ ] Observar y aprender versus desconectarse
  - [ ] Plan listo con antelación (según la fase de preparación)
- [ ] Extracción e identificación de las características del adversario
  - [ ] Identificación de otros sistemas afectados
  - [ ] Uso de firmas actualizadas del Sistema de Detección de Intrusiones de Red (NIDS), Sistema de Prevención de Intrusiones de Red (NIPS), Sistema de Detección de Intrusiones de Host (HIDS) y Sistema de Prevención de Intrusiones de Host (HIPS) o cualquier otra solución de seguridad disponible que permita evaluar los activos en todo el entorno.
    - [ ] Actualizar NIDS/NIPS/HIDS/HIPS u otra solución para buscar características:
      - [ ] Archivos
      - [ ] Llamadas del sistema
      - [ ] Procesos
      - [ ] Red
        - [ ] Puertos
        - [ ] Direcciones IP
        - [ ] Nombres de host
    - [ ] Realizar captura de paquetes (PCAP) y análisis forense de red para reproducir el tráfico e identificar sistemas infectados adicionales
- [ ] Realizar la identificación de qué esta siendo robado
  - [ ] Una captura completa de tráfico de red (PCAP) (que conserva una copia de todos los datos de la red) es invaluable en este sentido.
    - [ ] Incluso con un PCAP completo, es posible que el tráfico este cifrado.
    - [ ] Es necesario romper el cifrado para evaluar completamente el impacto.
    - [ ] Podría requerirse análisis forense del host junto al análisis de captura de tráfico para completar el análisis.
  - [ ] Propiedad intelectual
  - [ ] Recursos
    - [ ] Ancho de banda
- [ ] Identificar impacto legal y normativo
  - [ ] PCI
  - [ ] HIPAA
  - [ ] Leyes de protección de datos asociadas a cada país
  - [ ] Otros requerimientos normativos o legales a los cuáles la empresa este comprometida
- [ ] Aislamiento de toda el segmeneto de red
  - [ ] Se debe tener en cuenta que puede ser más fácil identificar el tráfico de red malicioso si el entorno sigue en línea, ya que el tráfico sigue fluyendo, pero podría haber una pérdida significativa de datos.
- [ ] Contacto con fuerzas del orden
  - [ ] Fuerzas locales encargados del manejo de ataques ciberneticos.
  - [ ] La decisión de involucrar a las fuerzas del orden puede afectar la visibilidad del incidente ante el público.
- [ ] Repote Público
  - [ ] Requerimientos normativos
  - [ ] Autoridades locales / internacionales
  - [ ] Notificación a cadena de suministro
  - [ ] Notificación a clientes
     
# Erradicación

- [ ] Recoplicación de todos los sistemas afectados y generación de imágenes forenses completas.
  - [ ] Las imágenes de memoria son muy importantes en el contexto de APTs, ya que algunas técnicas no se ejecutan en el disco duro.
    - [ ] También pueden ayudar en la evaluación de datos exfiltrados.
      - [ ] Si la exfiltración de datos utiliza cifrado simétrico, la clave de descifrado estará presente en la memoria de acceso aleatorio (RAM).
- [ ] Preferiblemente se deben incautar los discos duros como prueba y reemplazarlos con una nueva imagen del sistema que se encuentre limpia.
  - [ ] Revisar si es necesario custodiar pruebas legales recolectadas dentro del contexto del incidente.
  - [ ] Cualquier información de red o PCAP que pueda constituir una prueba válida dentro del proceso también debe conservarse.
    - [ ] Disponer de un procedimiento operativo estándar (POE) documentado para el manejo de la evidencia de red.
    - [ ] Asociar a la información de investigación del caso, generando un hash del PCAP almacenado.
- [ ] Una segunda opción es generar una imagen forense (posiblemente de forma remota), borrar las unidades y volver a crear la imagen.
- [ ] Sin esta evidencia, no se puede completar una investigación exhaustiva.
- [ ] Cerrar todos los vectores de exfiltración de red.
  - [ ] Inspección HTTPS mediante proxy e intercepción de Secure Socket Layer (SSL).
  - [ ] Prohibir la comunicación cifrada saliente, excepto para conexiones conocidas y autorizados.
  - [ ] Técnicas identificadas durante el análisis del APT.
- [ ] Cerrar todos los vectores de reinfección.
- [ ] Eliminar todos los RAT, C2 y puertas traseras.

# Recuperación

- [ ] Cerrar futuros vectores de exfiltración desde la red
  - [ ] Inspección HTTPS mediante proxy e intercepción SSL
- [ ] Prohibir la comunicación cifrada saliente, excepto para conexiones conocidas y autorizados.
- [ ] Rediseñar los sistemas para prevenir la reinfección
- [ ] Segmentar los datos críticos en áreas más restringidas
- [ ] Implementar controles de auditoría para el acceso a datos críticos
- [ ] Identificar a las personas dentro del entorno que, intencional o accidentalmente, contribuyeron al acceso de la APT, para su asesoramiento, capacitación y medidas disciplinarias

# Lecciones Aprendidas

- [ ] Evaluar la postura ejecutiva respecto a la gestión de incidentes y la seguridad de la información. ¿Esta pérdida es solo un costo de la actividad comercial o una oportunidad para un cambio radical?
- [ ] Desarrollar capacidades de inteligencia de amenazas para la identificación de ataques APT.
  - [ ] Caracterización del adversario.
    - [ ] Utilizar el modelo de "Kill Chain" u otras estrategias de inteligencia de amenazas.
    - [ ] En algunas ocasiones el adversario cuenta con recursos limitados y puede que llegue a reutilizar activos.
    - [ ] La atribución es muy difícil, pero es el objetivo final de las actividades de inteligencia de amenazas.
- [ ] Campaña para generación de consciencia a los miembros de la empresa ante diversos tipos de amenazas
  - [ ] Campañas de identificación de phishing
  - [ ] Analogías de Ataques
  - [ ] Explicar la posible pérdida de ventaja competitiva a largo plazo de la empresa debido a la pérdida de propiedad intelectual
- [ ] Recatalogar y revalorizar los activos en función de las estrategias y objetivos de las APT
  - [ ] Evitar la generación de culpas y aprovechar los incidentes para mejorar las capacidades
 - [ ] Mejora de métodos y capacidades de respuesta a las APT, incluyendo:
   - [ ] Capacidades de "observación y aprendizaje"
   - [ ] Capacidades de engaño (Cyber Deception)
     - [ ] Datos
     - [ ] Red
     - [ ] Host
- [ ] Agregación de datos de todas las fuentes
  - [ ] Gestión de eventos e información de seguridad (SIEM) si es posible
  - [ ] Identificar fuentes de datos adicionales
    - [ ] Firewalls
    - [ ] HIDS
    - [ ] Windows Active Directory (AD) / LDAP / Autenticación
    - [ ] Infraestructura inalámbrica
    - [ ] Cualquier sistema que no proporcione datos actualmente
      - [ ] Servidores
        - [ ] Servidores web
        - [ ] Servidores de bases de datos
      - [ ] Estaciones de trabajo
      - [ ] Dispositivos móviles
