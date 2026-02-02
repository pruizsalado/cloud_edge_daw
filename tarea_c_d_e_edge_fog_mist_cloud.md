# Tarea (c+d+e) · Edge, Fog, Mist y Cloud (DAW 1º)

## 🅲 Tarea C — Edge Computing y relación con Cloud
**Definición (3–5 líneas):**
Edge Computing es un modelo de computación donde el procesamiento de datos se realiza cerca del lugar donde estos se generan (dispositivos, sensores, gateways), en lugar de enviarlos todos a un centro de datos central. Su objetivo principal es reducir la latencia, optimizar el uso del ancho de banda y permitir respuestas en tiempo real. Es clave en entornos IoT, industriales y de tiempo crítico.

**Relación Edge ↔ Cloud (5–8 líneas):**
Edge Computing y Cloud Computing no se sustituyen, sino que se complementan. El edge se encarga del procesamiento inmediato y local de datos críticos, mientras que la nube centraliza el almacenamiento, análisis avanzado, machine learning y la gestión global del sistema. La nube también permite actualizar, monitorear y escalar los nodos edge. Esta arquitectura híbrida mejora el rendimiento, la eficiencia y la resiliencia de las aplicaciones modernas.

**Ejemplo real:**
En vehículos autónomos, el edge computing procesa en tiempo real datos de cámaras y sensores para tomar decisiones inmediatas (frenar, girar, evitar obstáculos). Al mismo tiempo, la nube se utiliza para entrenar modelos de inteligencia artificial, analizar grandes volúmenes de datos históricos y distribuir actualizaciones de software a los vehículos.

**Fuentes oficiales (mín. 2):**
- AWS – What is Edge Computing?
https://aws.amazon.com/what-is/edge-computing/
- Microsoft Azure – What is Edge Computing?
https://learn.microsoft.com/en-us/azure/architecture/guide/architecture-styles/edge-computing

## 🅳 Tarea D — Fog vs Mist (niveles y zonas de aplicación)
**Definición Fog (2–4 líneas):**
Fog Computing es una capa intermedia entre Edge y Cloud que extiende los servicios de la nube hacia la red. Se encarga de procesar, filtrar y agregar datos provenientes de múltiples nodos edge. Reduce la latencia y el tráfico hacia la nube, manteniendo cierta capacidad de análisis distribuido.

**Definición Mist (2–4 líneas):**
Mist Computing es el nivel más cercano a la fuente de datos, ubicado directamente en sensores y dispositivos IoT. Realiza procesamiento mínimo y decisiones muy simples en tiempo real. Su enfoque principal es la inmediatez y el consumo ultra bajo de recursos.

**Esquema (ASCII o Mermaid recomendado):**
graph TD
    A[Cloud<br/>Análisis global<br/>Big Data<br/>ML] 
    B[Fog<br/>Agregación<br/>Filtrado<br/>Coordinación]
    C[Edge<br/>Procesamiento local<br/>Control en tiempo real]
    D[Mist<br/>Sensores<br/>Actuadores]

    A --> B
    B --> C
    C --> D


**Zonas de aplicación (qué hace cada capa):**
- Mist → Lectura de sensores, filtrado básico, acciones inmediatas simples (ej. activar una alarma).
- Edge → Procesamiento local en tiempo real, control de dispositivos, análisis rápido de datos.
- Fog → Agregación de datos de múltiples edges, análisis intermedio, optimización del tráfico hacia la nube.
- Cloud → Almacenamiento masivo, análisis avanzado, inteligencia artificial, gestión y orquestación global.
