# RESPUESTAS — Reflexión y Resumen (Plantilla genérica)

> **Actividad / ID:**  2.a..e
> **Unidad / Tema:**  Unidad 2
> **Alumno/a:**  Manuel Maye Piulestan
> **Fecha:**  23/02/2026

---

## 1) Reflexión crítica (preguntas)
Responde con **lenguaje técnico** y **argumentos** (no solo opiniones). Si procede, usa ejemplos, riesgos y decisiones justificadas.

### 1.1) ¿Qué te han parecido los temas tratados en la unidad?
- Me parecén temas interesantes y utiles, temas como el OSINT pueden servir en varias ramas de la ciberseguridad dependiendo de como se enfoquen ya que en pentesting y red teaming tambien puede cambiar de ser un pentesting mediocre a uno en profundidad, tambien el tema de documentación aunque suele ser bastante tedioso es un tema bastante importante ya que analizar un incidente casi todos podemos hacerlo, pero hacer un reporting que tanto como altos cargos no ligados al sector IT y equipos de IT puedan entender requiere de un conocimiento que poca gente consigue obtener.

### 1.2) ¿Qué ha sido más útil para tu futuro puesto de trabajo? ¿Por qué?
- En mi caso, creo que lo mas útil para mi futuro ha sido el tema de OSINT y reporting ya que me quiero dedicar al pentesting/read team y sacar credenciales o información a base de OSINT puede ser decisivo para lograr penetrar el sistema, y el reporting para hacer un informe detallado y que tanto blue team como altos cargos, entiendan a que se enfrentan y lo que pueden perder.

### 1.3) ¿Qué partes ya conocías y cuáles han sido nuevas para ti?
- Conocia algunas herramientas de OSINT, como google dorking, TheHarvester, google images, shodan y sabia sacar información pero no de manera profesional y he aprendido a hacerlo de forma ordenada y con una metodologia correcta y recolección de pruebas para que sean validas para lo que sea.
- Todo el tema de las buenas practicas y consejos a la hora de hacer reporting son nuevas para mi y es algo que creo que he aprendido bastante.
- También el tema del SIEM no lo habia tocado nunca, la creación de pipelines para el flujo de datos desde el servicio el envio de la información por parte de filebeat, a logstash y luego a elasticsearch, a configuración de snort.

### 1.4) ¿Qué concepto/idea te ha llamado más la atención y por qué?
- El concepto de SIEM ya que no sabía de su existencia antes de estudiar esto y me parece que es una idea bastante buena ya que la centralizacion de los logs y su sistema de alertas, puede prevenir muchos ataques

### 1.5) ¿Qué parte recortarías o simplificarías si hubiera menos tiempo? Justifica.
- A parte de lo que ya he mencionado del SIEM, no recortaria nada ya que creo que todo lo visto es importante y necesario para tener una buena base de conocimientos en el sector, aunque si tuviera que recortar algo, recortaria un poco el tema de OSINT ya que aunque es un tema muy interesante, creo que se podria haber dado un poco mas por encima y centrarse mas en el reporting y el SIEM que son temas mas complejos y con mas profundidad.

### 1.6) ¿Qué tema has echado en falta o ampliarías? Justifica.
- El tema del SIEM lo cambiaria por un uso real de un SOC con honeypots para analizar las alertas de manera realista  y no un POC como hemos hecho en clase ya que a mi parecer, he perdido más tiempo en que funcione bien y no en analizar las alertas y los logs centralizados.

### 1.7) ¿Qué aplicarías “mañana” en un entorno real con recursos limitados?
- Un SIEM basico para los servicios criticos de la empresa, con algunas pipelines basicas, ya que, podemos ganar muchisimo control e incluso reducir gastos ya que, en vez de ir servicio por servicio perdiendo horas y horas de revisiones de logs, al tener todo centralizado solo se veria en un unico equipo.

### 1.8) ¿Qué duda, riesgo o punto crítico te queda abierto tras la unidad?
- La duda de como se podria llegar a gestionar de forma eficiente un SIEM con logs de muchos servicios distintos.


## 2) Resumen esquematizado (obligatorio)

**Resumen general:** Esta unidad ha cubierto todo el ciclo de gestión de incidentes de ciberseguridad:

```
┌─────────────────────────────────────────────────────────────────┐
│  CLASIFICACIÓN → DETECCIÓN → INVESTIGACIÓN → DOCUMENTACIÓN     │
└─────────────────────────────────────────────────────────────────┘

1️⃣ TAXONOMÍA Y CLASIFICACIÓN
   → 5 dimensiones (C-I-T-A-D) → 3 niveles (BAJO/MEDIO/ALTO)
   → 10 categorías de incidentes INCIBE/ENISA
   → Determinar categoría del sistema (BÁSICA/MEDIA/ALTA)

2️⃣ DETECCIÓN EN EL SOC
   → IDS (detecta) vs IPS (detecta + bloquea)
   → SIEM: centraliza logs, correlaciona, alerta
   → Casos de uso para cada amenaza
   → Evolución: SIEM → SOAR (automatización)

3️⃣ INVESTIGACIÓN CON OSINT
   → Proceso: Planificar → Identificar → Adquirir → Procesar → Analizar → Difundir
   → Herramientas: Shodan, Maltego, TheHarvester, HIBP
   → Solo fuentes públicas (legal y ético)

4️⃣ DOCUMENTACIÓN
   → Ciclo: Preparación → Identificación → Contención → Erradicación → Recuperación → Lecciones
   → Informe: Resumen ejecutivo (1 pág) + Cuerpo + Anexos técnicos
   → Vector → Técnica → Vulnerabilidad → Impacto
```

### 2.1) Mapa/índice de la unidad (visión global)

```
UNIDAD 2: GESTIÓN DE INCIDENTES DE CIBERSEGURIDAD

├── 2.1 CLASIFICACIÓN Y TAXONOMÍA
│   ├─ Dimensiones de seguridad (C-I-T-A-D)
│   ├─ Categorías ENS (BÁSICA/MEDIA/ALTA)
│   └─ Taxonomía INCIBE (10 categorías)
│
├── 2.2 DETECCIÓN Y SOC
│   ├─ IDS/IPS
│   ├─ SIEM (recopilación, correlación, alertas)
│   ├─ Casos de uso
│   └─ Evolución SOAR
│
├── 2.3 OSINT
│   ├─ Proceso (6 fases)
│   ├─ Técnicas (Google Dorking, metadatos)
│   └─ Herramientas (Shodan, Maltego, HIBP)
│
└── 2.4 DOCUMENTACIÓN
    ├─ Ciclo de vida del incidente
    ├─ Estructura de informes
    └─ Vectores de ataque
```

### 2.2) Conceptos clave (lista breve)

- **Incidente de seguridad**: Suceso que afecta a Confidencialidad, Integridad o Disponibilidad
- **5 Dimensiones de seguridad**: Confidencialidad, Integridad, Trazabilidad, Autenticidad, Disponibilidad (C-I-T-A-D)
- **Categorías ENS**: BÁSICA, MEDIA, ALTA (según impacto en las dimensiones)
- **Taxonomía INCIBE**: 10 categorías (Contenido abusivo, Código dañino, Obtención info, Intento/Intrusión, Disponibilidad, Seguridad info, Fraude, Vulnerable, Otros)
- **Peligrosidad vs Impacto**: Capacidad del ataque vs daño real causado
- **SOC**: Centro de operaciones 24/7 para detectar, responder y prevenir
- **CERT/CSIRT**: Equipos de respuesta a incidentes críticos
- **IDS vs IPS**: Detecta y alerta vs Detecta y bloquea
- **SIEM**: Centraliza logs, correlaciona eventos, genera alertas en tiempo real
- **SOAR**: Automatización y orquestación de respuesta a incidentes
- **OSINT**: Inteligencia de fuentes públicas (no invasivo, legal)
- **IOC**: Indicadores de Compromiso (IPs, hashes, dominios maliciosos)
- **Vector de ataque**: Canal por donde entra (email, RDP, web, USB, Wi-Fi)
- **Técnica de ataque**: Método usado (phishing, fuerza bruta, SQLi, malware)

### 2.3) Procesos / procedimientos (pasos o checklist)

**Ciclo de vida de gestión de incidentes**
1. Preparación → 2. Identificación → 3. Contención → 4. Erradicación → 5. Recuperación → 6. Lecciones aprendidas

**Proceso OSINT**
1. Planificación → 2. Identificación de fuentes → 3. Adquisición → 4. Procesamiento → 5. Análisis → 6. Difusión

**Fases de implementación SIEM**
1. Descubrimiento (planificar) → 2. Piloto (probar casos de uso) → 3. Implementación (desplegar) → 4. Mejora continua (actualizar)

**Análisis de incidente (Vector-Técnica-Vulnerabilidad-Impacto)**
- Vector: ¿Por dónde? → Técnica: ¿Cómo? → Vulnerabilidad: ¿Por qué funcionó? → Impacto: ¿Qué consiguió?

### 2.4) Herramientas / técnicas (si aplica)

**Detección y Monitorización**
- **IDS/IPS**: Snort, Suricata
- **SIEM comerciales**: Splunk, QRadar, ArcSight, LogRhythm
- **SIEM open source**: ELK Stack (Elasticsearch + Logstash + Kibana)
- **Agentes de logs**: Filebeat, Logstash

**OSINT - Reconocimiento**
- **Motores búsqueda**: Google Dorking
- **Dominios/IPs**: WHOIS, Shodan, Censys, VirusTotal
- **Redes sociales**: Sherlock (buscar usuarios en múltiples plataformas), TheHarvester (emails)
- **Filtraciones**: Have I Been Pwned, DeHashed, BreachDirectory
- **Metadatos**: FOCA, ExifTool, metagoofil
- **Histórico web**: Wayback Machine (archive.org)
- **Dark web**: Tor Browser, OnionScan

**Documentación**
- Procesadores de texto con plantillas predefinidas
- Plataformas colaborativas: Confluence, Notion, SharePoint

### 2.5) Buenas prácticas y errores típicos

**Buenas prácticas**

✅ **En detección y SOC**
- Definir casos de uso claros ANTES de implementar el SIEM
- Priorizar fuentes de logs críticas (no monitorizar todo desde el día 1)
- Mantener runbooks actualizados para cada tipo de incidente
- Revisar y actualizar reglas del SIEM regularmente (eliminar falsos positivos)
- Implementar niveles de analistas (Nivel 1, 2 y 3) para escalar eficientemente

✅ **En OSINT**
- Usar metodología estructurada (no recopilar datos sin criterio)
- Verificar la fiabilidad de las fuentes antes de confiar en ellas
- Respetar límites legales y éticos (solo información pública)
- Documentar las fuentes y métodos usados (reproducibilidad)

✅ **En documentación**
- Documentar desde el minuto 1, no al final del incidente
- Usar plantillas para ahorrar tiempo y estandarizar
- Resumen ejecutivo de máximo 1 página para jefes
- Evidencias técnicas extensas van en anexos
- Pasar SIEMPRE el corrector ortográfico antes de enviar
- Frases cortas y párrafos de máximo 6-8 líneas

**Errores típicos**

❌ **En detección y SOC**
- Implementar SIEM sin casos de uso definidos (no sabes qué buscar)
- Enviar todos los logs sin filtrar (genera ruido y cuesta más)
- No ajustar umbrales de alertas (fatiga por falsos positivos)
- No tener runbooks/playbooks (improvisación ante incidentes)

❌ **En OSINT**
- Recopilar información sin objetivo claro (pérdida de tiempo)
- Confiar ciegamente en cualquier fuente sin verificar
- Cruzar la línea legal (acceso no autorizado, suplantar identidades)
- No documentar las fuentes consultadas

❌ **En documentación**
- Informes kilométricos con relleno innecesario (saturación cognitiva)
- Faltas de ortografía (destroza credibilidad del informe)
- Frases de 8 líneas imposibles de leer
- Mezclar evidencias técnicas extensas en el cuerpo (usar anexos)

### 2.6) Glosario mínimo (términos y definiciones cortas)

- **DNS (Domain Name System)**: Sistema que traduce nombres de dominio a IPs
- **EDR (Endpoint Detection & Response)**: Herramienta de detección en endpoints
- **EPS (Events Per Second)**: Eventos por segundo que procesa un SIEM
- **Exploit**: Código que aprovecha una vulnerabilidad para comprometer un sistema
- **Firewall**: Dispositivo que filtra tráfico de red según reglas
- **Hash**: Huella digital única de un archivo (MD5, SHA1, SHA256)
- **IDS (Intrusion Detection System)**: Sistema de detección de intrusiones (solo alerta)
- **IOA (Indicators of Attack)**: Indicadores de ataque (tácticas y técnicas usadas)
- **IOC (Indicators of Compromise)**: Indicadores de compromiso (IPs, hashes, dominios maliciosos)
- **IPS (Intrusion Prevention System)**: Sistema de prevención de intrusiones (alerta y bloquea)
- **MFA (Multi-Factor Authentication)**: Autenticación de múltiples factores
- **Ransomware**: Malware que cifra archivos y pide rescate
- **SIEM (Security Information & Event Management)**: Plataforma centralizada de gestión de logs y eventos de seguridad
- **SOAR (Security Orchestration, Automation & Response)**: Herramienta para automatizar respuesta a incidentes
- **SOC (Security Operations Center)**: Centro de operaciones de seguridad que monitorea 24/7
- **Syslog**: Protocolo estándar para enviar logs de red
- **VPN (Virtual Private Network)**: Red privada virtual para acceso remoto seguro
- **WHOIS**: Base de datos pública de propietarios de dominios


## 3) (Opcional) Evidencias y recursos usados
Enlaza aquí evidencias (capturas, logs, configuraciones, salidas de comandos, etc.) si forman parte de tu trabajo.

### Evidencia 1
- Archivo: `evidencias/nginx-snort.conf`
- Qué demuestra: El uso de pipelines para centralizar logs en un SIEM y la división en diferentes pipelines para cada servicio, en este caso, nginx y snort.
- Qué he aprendido: A configurar pipelines para centralizar logs en un SIEM, y la importancia de dividir los pipelines por servicio para una mejor organización y análisis de los logs.

### Evidencia 2
- Archivo: `evidencias/snort.conf`
- Qué demuestra: Configuración de reglas de detección de amenazas en Snort.
- Qué he aprendido: A configurar reglas personalizadas en Snort para detectar amenazas específicas y analizar alertas generadas por el sistema.


## 4) Conclusión (cierre)
Esta unidad me ha dado una visión completa de cómo funciona la gestión de incidentes de seguridad en el mundo real. Lo que más me ha quedado claro es que todo está conectado: no vale solo detectar un ataque con un SIEM si luego no sabes clasificarlo bien, investigarlo con OSINT y documentarlo correctamente para aprender de él.

El SIEM me parece una herramienta brutal porque centraliza todo, pero también he visto que no es plug&play: hay que pensar bien qué logs meter, crear casos de uso y ajustar alertas para no morir con falsos positivos. Lo del OSINT me ha sorprendido bastante, no sabía que se podía sacar tanta información útil solo de fuentes públicas sin hacer nada ilegal.

Y sobre la documentación, aunque es la parte más rollo, entiendo que es clave. Un incidente sin documentar es un incidente del que no aprendes nada, y si no tienes un informe bien hecho cuando te lo pidan (tu jefe, un auditor o hasta en un juicio), estás vendido.

En resumen, esta unidad me ha dado herramientas muy útiles para trabajar en ciberseguridad, ya sea en un SOC, haciendo pentesting o respondiendo a incidentes. Clasificar, detectar, investigar y documentar: las cuatro patas de una buena gestión de incidentes.