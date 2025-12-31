# Análisis de Gestión de Activos - Oficina en Casa

## Introducción
Este proyecto documenta el inventario de activos de red para una pequeña empresa operada desde el hogar. El objetivo es identificar dispositivos, evaluar sus características y clasificar su sensibilidad para priorizar esfuerzos de seguridad.

## Inventario de Activos

| Activo | Acceso | Propietario | Ubicación | Sensibilidad |
| :--- | :--- | :--- | :--- | :--- |
| Network router | Continuo | ISP | On-premises | Confidential |
| Desktop | Occasional | Homeowner | On-premises | Restricted |
| Guest smartphone | Occasional | Friend | On/Off-premises | Internal-only |
| **Laptop corporativa** | Continuo | Propietario | Oficina | **Restricted** |
| **Servidor NAS** | Continuo | Propietario | Oficina | **Confidential** |
| **Impresora Wi-Fi** | Occasional | Propietario | Oficina | **Internal-only** |

## Criterios de Clasificación
Para la asignación de sensibilidad, se utilizaron los siguientes niveles basados en el impacto al negocio:

1.  **Restricted (Restringido):** Información crítica cuya divulgación causaría daños graves (ej. datos financieros). Acceso bajo "necesidad de saber".
2.  **Confidential (Confidencial):** Datos sensibles para el funcionamiento interno. Acceso limitado a usuarios específicos.
3.  **Internal-only (Solo Interno):** Información para todos los miembros de la red doméstica. No destinada al público.
4.  **Public (Público):** Información que no causa daño si es vista por cualquier persona.

## Notas de Seguridad
- Se identificó que la **Laptop corporativa** requiere medidas adicionales como cifrado de disco y MFA.
- El **Servidor NAS** debe estar segmentado en la red para evitar que invitados (Guest smartphone) puedan alcanzarlo.
