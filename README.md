# TSI-203 Seguridad de Redes
## Infraestructura 1 – VPN Site-to-Site

**Estudiante:** Jennifer López  
**Matrícula:** 20240860  

## 🎥 Video de demostración

🔗 **Enlace:** Pendiente de agregar

---

## Objetivo

Implementar una infraestructura de Seguridad de Redes utilizando dos
firewalls FortiGate conectados mediante una VPN Site-to-Site.

La infraestructura permite la comunicación segura entre la red de
usuarios y la red de servidores a través de un túnel VPN.

## Características principales

- 2 FortiGate
- VPN Site-to-Site
- IKEv2
- Cifrado AES256-SHA256
- Red de usuarios /25
- Red de servidores /28
- Direccionamiento WAN público simulado
- Rutas estáticas a través del túnel VPN
- Pruebas de conectividad entre ambas redes

## Direccionamiento

| Segmento | Dirección |
|---|---|
| Red de usuarios | 10.86.0.0/25 |
| Gateway usuarios | 10.86.0.1 |
| PC usuario | 10.86.0.10 |
| Red de servidores | 10.86.1.0/28 |
| Gateway servidores | 10.86.1.1 |
| Servidor | 10.86.1.2 |
| WAN FGT-USUARIO | 200.20.86.1 |
| WAN FGT-SERVIDOR | 200.20.86.2 |

## VPN Site-to-Site

La VPN fue configurada entre ambos FortiGate utilizando los siguientes
parámetros principales:

- IKE Version: IKEv2
- Encryption: AES256
- Authentication: SHA256
- Tipo: Route-Based VPN
- Autenticación mediante Pre-Shared Key

## Validación

Durante las pruebas se verificó:

- Comunicación entre ambos peers.
- Establecimiento del túnel VPN.
- Comunicación entre la red USER y SERVER.
- Rutas estáticas mediante la interfaz VPN.
- Pruebas de ping entre los extremos.
- Prueba de traceroute.
- Comportamiento de la comunicación al deshabilitar y habilitar la ruta VPN.

## Documentación

La documentación técnica completa de la infraestructura se encuentra
disponible dentro de este repositorio.

## Evidencias

El repositorio contiene las evidencias utilizadas para demostrar la
configuración y funcionamiento de la infraestructura.
