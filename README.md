# NETSHIELD
Infraestructura de redes segura para PYMES

## Descripción
Solución completa que dispone de una seguridad continua  en toda nuestra infraestructura y ofrece una mayor facilidad a la hora de realizar servicios de gestión de red y usuarios, detección y bloqueo de amenazas, centralización de almacenamiento, conexión remota mediante VPN y monitorización del estado de la red.

## Tecnologías 

### pfSense | WireGuard | Suricata | Windows Server | Nextcloud | Prometheus | Loki | Grafana | Flask | RAID

**pfSense** - 
Firewall, DHCP, DNS, segmentación mediante VLAN y conectividad de la red.

**WireGuard** - 
VPN para acceso remoto seguro de usuarios autorizados.

**Suricata** - 
Detección de posibles intrusiones y prevención según las reglas y el modo configurado.

**Windows Server** - 
Dominio, autenticación, cuentas, grupos y permisos.

**Nextcloud** - 
Almacenamiento centralizado y gestión de archivos.

**Python y Flask** - 
Desarrollo del panel web personalizado.

**Prometheus** - 
Recogida y almacenamiento de métricas de los sistemas instrumentados.

**Loki y Grafana** - 
Consulta de registros y visualización de métricas y logs.

**RAID y copias de seguridad** - 
Redundancia ante ciertos fallos de disco y recuperación de información; RAID no sustituye las copias.



## Arquitectura

La red se divide en cuatro VLANs:

| VLAN | Uso | Red |
|---|---|---|
| 10 | Servidores | 192.168.10.0/24 |
| 20 | Usuarios y clientes | 192.168.20.0/24 |
| 30 | Gestión | 192.168.30.0/24 |
| 40 | Invitados | 192.168.40.0/24 |

Los diagramas de red y de servicios están en la carpeta `docs/`.

## Estructura del repositorio

```
docs/             Documentación, diagramas y planificación
network/          pfSense: DHCP, DNS, VLANs y firewall
vpn/              WireGuard
ids/              Suricata
windows-server/   Dominio y permisos
nextcloud/        Almacenamiento y copias de seguridad
monitoring/       Prometheus, Loki y Grafana
web/              Panel web en Flask
scripts/          Scripts de despliegue y pruebas
```

## Estado del proyecto

En desarrollo. Actualmente en fase de preparación del entorno

## Autores
Iker Nohales | Daniel Avilés
