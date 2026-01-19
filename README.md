# # Tarea (a+b) · Cloud: niveles y funciones (DAW 1º)

ENLACE AL REPOSITORIO DE GITHUB: [https://github.com/pruizsalado/cloud_edge_daw/blob/tarea/cloud-a-b/README.md](https://github.com/pruizsalado/cloud_edge_daw/blob/tarea/cloud-a-b/README.md)

## 🅰️ Tarea A — Niveles de cloud (IaaS/PaaS/SaaS)
Crea una tabla con 10 servicios reales. Incluye enlace oficial y justifica responsabilidades.

| **Servicio**               | **Proveedor**       | **Nivel (IaaS/PaaS/SaaS)** | **Enlace oficial**                                                                                                           | **¿Qué gestiona el proveedor?**                               | **¿Qué gestiona el equipo/usuario?**                                 |
| -------------------------- | ------------------- | -------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------- | -------------------------------------------------------------------- |
| **Amazon EC2**             | AWS                 | IaaS                       | [https://aws.amazon.com/ec2/](https://aws.amazon.com/ec2/)                                                                   | Infraestructura física, virtualización, red y almacenamiento. | SO, apps, datos, seguridad OS y configuraciones.                     |
| **Google Compute Engine**  | Google Cloud        | IaaS                       | [https://cloud.google.com/compute](https://cloud.google.com/compute)                                                         | Hardware, red, virtualización y mantenimiento.                | SO, servicios instalados y datos.                                    |
| **Azure Virtual Machines** | Microsoft Azure     | IaaS                       | [https://azure.microsoft.com/en-us/services/virtual-machines/](https://azure.microsoft.com/en-us/services/virtual-machines/) | Infraestructura base y virtualización.                        | OS, apps, datos y parches de software.                               |
| **OpenStack**              | Open Infrastructure | IaaS*                      | [https://www.openstack.org/](https://www.openstack.org/)                                                                     | Infraestructura de nube y virtualización.                     | Administrar VMs, redes, almacenamiento (si se usa). ([Wikipedia][1]) |
| **Google App Engine**      | Google Cloud        | PaaS                       | [https://cloud.google.com/appengine](https://cloud.google.com/appengine)                                                     | Infraestructura, runtime, escalado y servicios base.          | Código de app, configuración y datos.                                |
| **AWS Elastic Beanstalk**  | AWS                 | PaaS                       | [https://aws.amazon.com/elasticbeanstalk/](https://aws.amazon.com/elasticbeanstalk/)                                         | Plataforma de despliegue, aprovisionamiento y balanceo.       | Código, configuración de despliegue y datos. ([Wikipedia][2])        |
| **Heroku**                 | Salesforce          | PaaS                       | [https://www.heroku.com/](https://www.heroku.com/)                                                                           | Plataforma completa para ejecutar apps, runtime.              | Código, configuración y add-ons. ([Wikipedia][3])                    |
| **Google Workspace**       | Google              | SaaS                       | [https://workspace.google.com/](https://workspace.google.com/)                                                               | Infraestructura, app completa, actualizaciones y seguridad.   | Cuentas de usuario, datos y configuración.                           |
| **Microsoft 365**          | Microsoft           | SaaS                       | [https://www.microsoft.com/microsoft-365](https://www.microsoft.com/microsoft-365)                                           | Software app, mantenimiento, parches y backups.               | Contenidos, usuarios y configuración.                                |
| **Salesforce CRM**         | Salesforce          | SaaS                       | [https://www.salesforce.com/](https://www.salesforce.com/)                                                                   | Aplicación CRM completa, infraestructura y ops.               | Datos de clientes y personalizaciones. ([IBM][4])                    |

## 🅱️ Tarea B — Funciones principales de cloud (arquitectura)
Incluye un diagrama (ASCII/Mermaid/imagen) y una explicación breve.

### Diagrama
```
      |Usuario|
         |
         v
     |Frontend|
         |
         v
   |Load Balancer|
         |
         v
      |Compute|
      (Servidor)
      /       \
 |Storage|    |Database|
```

### Explicación (8–12 líneas)
(Describe el flujo front → API → BBDD/storage y dónde entra la cloud)

-El usuario accede a la aplicación desde el frontend (web o app).

-El frontend envía las solicitudes a la API alojada en la nube.

-La API se ejecuta en servicios de cómputo cloud, como servidores o contenedores.

-Un balanceador de carga distribuye las peticiones para evitar sobrecargas.

-La lógica de la aplicación procesa la información recibida.

-Cuando es necesario, la API consulta o guarda datos en la base de datos.

-Los archivos se almacenan en servicios de storage en la nube.

-La cloud permite escalar recursos según la demanda.

-También ofrece alta disponibilidad y tolerancia a fallos.

-De esta forma, el sistema es seguro, flexible y eficiente.

### Mapeo de funciones cloud a componentes (mínimo 3)

- **Procesamiento** → Compute / Servidores / Contenedores  
  *(Se encarga de procesar la lógica de la aplicación y responder a solicitudes)*
- **Ejecución** → API / Serverless Functions  
  *(Ejecuta funciones específicas bajo demanda, sin necesidad de gestionar servidores completos)*
- **Almacenamiento** → Storage / Base de datos (Database)  
  *(Guarda archivos, documentos y datos estructurados de forma segura y escalable)*
- **Intercambio** → Load Balancer / CDN (opcional)  
  *(Distribuye solicitudes y contenido para optimizar rendimiento y disponibilidad)*

## 📚 Fuentes (enlaces oficiales)
(Enlaces oficiales usados en la tabla A y en la B)
## Referencias / Fuentes oficiales

- **Definición de Cloud Computing (NIST)**:  
  [https://nist.gov/publications/nist-definition-cloud-computing](https://www.nist.gov/publications/nist-definition-cloud-computing)

- **Qué es Cloud Computing (AWS)**:  
  [https://aws.amazon.com/what-is-cloud-computing/](https://aws.amazon.com/what-is-cloud-computing/)

- **Definición de Cloud Computing (Microsoft Azure)**:  
  [https://azure.microsoft.com/en-us/resources/cloud-computing-dictionary/what-is-cloud-computing/](https://azure.microsoft.com/en-us/resources/cloud-computing-dictionary/what-is-cloud-computing/)

- **Computación en la nube (Wikipedia en español)**:  
  [https://es.wikipedia.org/wiki/Computaci%C3%B3n_en_la_nube](https://es.wikipedia.org/wiki/Computaci%C3%B3n_en_la_nube)

- **Infraestructura como servicio – IaaS (Wikipedia en español)**:  
  [https://es.wikipedia.org/wiki/Infraestructura_como_servicio](https://es.wikipedia.org/wiki/Infraestructura_como_servicio)

- **Almacenamiento en nube (Wikipedia en español)**:  
  [https://es.wikipedia.org/wiki/Almacenamiento_en_nube](https://es.wikipedia.org/wiki/Almacenamiento_en_nube)

  Otras fuentes:
  - **"OpenStack"**:
   [https://en.wikipedia.org/wiki/OpenStack?utm_source=chatgpt.com](https://en.wikipedia.org/wiki/OpenStack?utm_source=chatgpt.com).
 - **"AWS Elastic Beanstalk"**:
   [https://es.wikipedia.org/wiki/AWS_Elastic_Beanstalk?utm_source=chatgpt.com](https://es.wikipedia.org/wiki/AWS_Elastic_Beanstalk?utm_source=chatgpt.com).
    - **"Heroku"**:
   [https://es.wikipedia.org/wiki/Heroku?utm_source=chatgpt.com](https://es.wikipedia.org/wiki/Heroku?utm_source=chatgpt.com).
 - **"Iaas, Paas, Saas: ¿cuál es la diferencia? | IBM"**:
   [https://www.ibm.com/es-es/think/topics/iaas-paas-saas?utm_source=chatgpt.com](https://www.ibm.com/es-es/think/topics/iaas-paas-saas?utm_source=chatgpt.com).

