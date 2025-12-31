#  Gestión de Activos de Red: Inventario y Clasificación de Seguridad

Este repositorio contiene un proyecto práctico de **Gestión de Activos (Asset Management)** enfocado en la seguridad de una oficina doméstica (*home office*). El objetivo principal es identificar, documentar y clasificar los dispositivos conectados a una red para mitigar riesgos y priorizar la protección de la información.

##  Descripción del Proyecto

En el ámbito de la ciberseguridad, no se puede proteger lo que no se conoce. Este proyecto simula la gestión de activos para una pequeña empresa que opera desde casa. Se ha creado un inventario detallado que evalúa la importancia de cada dispositivo basándose en la sensibilidad de los datos que maneja y su función dentro de la red.

### Objetivos:
* **Identificar** todos los puntos de entrada potenciales a la red doméstica.
* **Documentar** características clave como propiedad, ubicación y tipo de acceso.
* **Clasificar** los activos según niveles de sensibilidad (Confidencial, Restringido, Interno, Público).
* **Evaluar riesgos** específicos asociados a cada dispositivo.

---

##  Estructura del Repositorio

* `/data`: Contiene el inventario en formatos `.xlsx` y `.csv`.
* `/docs`: Documentación detallada del análisis y metodología de clasificación.
* `README.md`: Descripción general del proyecto (este archivo).

---

##  Resumen del Inventario

A continuación, se muestra una vista previa de los activos analizados:

| Activo | Propietario | Sensibilidad | Notas de Seguridad |
| :--- | :--- | :--- | :--- |
| **Laptop Corporativa** | Propietario | **Restricted** | Datos bancarios y de clientes. Uso de VPN obligatorio. |
| **Network Router** | ISP | **Confidential** | Punto central de control. Doble frecuencia (2.4/5GHz). |
| **Servidor NAS** | Propietario | **Confidential** | Backups y archivos históricos. Acceso limitado. |
| **Desktop** | Dueño de casa | **Restricted** | Contiene información privada y fotos sensibles. |
| **Impresora Wi-Fi** | Propietario | **Internal-only** | Riesgo de acceso lateral si no se actualiza el firmware. |
| **Guest Smartphone** | Invitado | **Internal-only** | Acceso temporal. Segmentado de la red principal. |

---

##  Metodología de Clasificación

Para este análisis, se utilizó la siguiente escala de sensibilidad:

1.  **Restricted (Restringido):** Información crítica cuya pérdida causaría daños graves. Acceso basado estrictamente en la necesidad de saber.
2.  **Confidential (Confidencial):** Información sensible para el negocio. Acceso limitado a usuarios autorizados.
3.  **Internal-only (Solo Interno):** Datos destinados únicamente para el uso dentro de la organización/red del hogar.
4.  **Public (Público):** Información que no representa un riesgo si es accedida por externos.

---

##  Conclusiones

La realización de este inventario permitió identificar que la **Laptop Corporativa** y el **Servidor NAS** son los activos que requieren controles de seguridad más estrictos (como cifrado y autenticación de múltiples factores). Este proyecto demuestra la importancia de la visibilidad de activos como el primer paso en cualquier estrategia de defensa en profundidad.

---
**Autor:** [Angel Josue Hernandez Marmolejo]  
**Curso:** Google Cybersecurity Professional Certificate (Práctica de Inventario)
