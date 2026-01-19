# # Tarea (a+b) · Cloud: niveles y funciones (DAW 1º)

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

[1]: https://en.wikipedia.org/wiki/OpenStack?utm_source=chatgpt.com "OpenStack"
[2]: https://es.wikipedia.org/wiki/AWS_Elastic_Beanstalk?utm_source=chatgpt.com "AWS Elastic Beanstalk"
[3]: https://es.wikipedia.org/wiki/Heroku?utm_source=chatgpt.com "Heroku"
[4]: https://www.ibm.com/es-es/think/topics/iaas-paas-saas?utm_source=chatgpt.com "Iaas, Paas, Saas: ¿cuál es la diferencia? | IBM"

## 🅱️ Tarea B — Funciones principales de cloud (arquitectura)
Incluye un diagrama (ASCII/Mermaid/imagen) y una explicación breve.

### Diagrama
(Pega aquí el diagrama)

### Explicación (8–12 líneas)
(Describe el flujo front → API → BBDD/storage y dónde entra la cloud)

### Mapeo de funciones cloud a componentes (mínimo 3)
- Procesamiento → …
- Ejecución → …
- Almacenamiento → …
- Intercambio → … (opcional si ya tienes 3)

## 📚 Fuentes (enlaces oficiales)
(Enlaces oficiales usados en la tabla A y en la B)
