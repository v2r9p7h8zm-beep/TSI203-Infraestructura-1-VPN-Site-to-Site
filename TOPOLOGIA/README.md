# Topología – Infraestructura 1

La Infraestructura 1 fue desarrollada en GNS3 y está compuesta por dos FortiGate conectados a través de una red WAN/ISP simulada.

## Segmentos principales

**USER**
- Red: 10.86.0.0/25
- Gateway: 10.86.0.1
- PC-USUARIO: 10.86.0.10

**SERVER**
- Red: 10.86.1.0/28
- Gateway: 10.86.1.1
- PC-SERVIDOR: 10.86.1.2

**WAN**
- FGT-USUARIO: 200.20.86.1
- FGT-SERVIDOR: 200.20.86.2

La comunicación entre las redes USER y SERVER se realiza mediante el túnel VPN Site-to-Site `VPN-SITE`.
