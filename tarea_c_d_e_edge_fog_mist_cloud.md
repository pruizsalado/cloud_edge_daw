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

<pre>
Cloud
  ↑  análisis global / IA
Fog
  ↑  agregación / filtrado
Edge
  ↑  procesamiento local
Mist
  ↑  sensores / actuadores
</pre>


**Zonas de aplicación (qué hace cada capa):**
- Mist → Lectura de sensores, filtrado básico, acciones inmediatas simples (ej. activar una alarma).
- Edge → Procesamiento local en tiempo real, control de dispositivos, análisis rápido de datos.
- Fog → Agregación de datos de múltiples edges, análisis intermedio, optimización del tráfico hacia la nube.
- Cloud → Almacenamiento masivo, análisis avanzado, inteligencia artificial, gestión y orquestación global.

## 🅴 Tarea E — Ventajas de la Cloud en sistemas conectados
Incluye mínimo 3 ventajas (recomendado 5), con explicación + ejemplo.

1) Ventaja: Escalabilidad
   Explicación: La nube permite aumentar o reducir recursos (cómputo, almacenamiento, red) de forma dinámica según la demanda, sin necesidad de cambiar la infraestructura física. Esto es clave en sistemas conectados con cargas variables.
   Ejemplo: Una plataforma IoT puede gestionar miles de sensores adicionales durante horas pico sin interrupciones, escalando automáticamente los servicios en la nube.

2) Ventaja: Alta disponibilidad
   Explicación: Los proveedores cloud ofrecen infraestructura distribuida geográficamente con mecanismos de redundancia y tolerancia a fallos, garantizando que los sistemas estén disponibles incluso ante fallos.
   Ejemplo: Un sistema de monitoreo industrial sigue funcionando aunque un centro de datos tenga una caída, gracias a la replicación en múltiples regiones.

3) Ventaja: Procesamiento y análisis avanzado
   Explicación: La nube facilita el uso de Big Data, analítica avanzada e inteligencia artificial para procesar grandes volúmenes de datos provenientes de dispositivos conectados.
   Ejemplo: Datos recopilados por sensores de tráfico se analizan en la nube para predecir congestiones y optimizar semáforos mediante modelos de IA.

4) Ventaja: Reducción de costos
   Explicación: El modelo de pago por uso elimina la necesidad de grandes inversiones iniciales en hardware y mantenimiento, optimizando el costo total del sistema.
   Ejemplo: Una startup de smart cities paga solo por los recursos cloud utilizados durante pruebas y despliegues, sin comprar servidores propios.

5) Ventaja: Gestión centralizada
   Explicación: La nube permite administrar, monitorear y actualizar dispositivos conectados desde un único punto, simplificando la operación del sistema.
   Ejemplo: Actualizaciones de firmware para miles de dispositivos IoT se distribuyen remotamente desde la nube.

**Fuente oficial (mín. 1):**
- Amazon Web Services (AWS) — Benefits of Cloud Computing
https://aws.amazon.com/what-is-cloud-computing/

