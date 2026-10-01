# Practica.II-VPN-Fortigate-a-Fortigate

Enlace del video
https://youtu.be/deTagFvhInU

<img width="2186" height="1952" alt="P2-Fortinet a Fortinet" src="https://github.com/user-attachments/assets/547f0adc-da7e-44d8-9f4d-1fef3d37968e" />

## I. Direccionamiento IP

En este apartado estaré mostrando el direccionamiento IP, utilizado en la topología, se realizó un VLSM que tenga dígitos similares a mi matricula (2025-0863), y el direccionamiento es el siguiente:

| Nombre Red | Dispositivos | Primera Interfaz | Ultima Interfaz |
|---|---|---|---|
| Red Publica 192.8.63.0/24 | Fortigate1 – Fortigate2 | 192.8.63.200 | 192.8.63.201 |
| VLAN 10 (Usuarios) 172.8.63.0/25 | Interfaz - Usuario | 172.8.63.1 | DHCP |
| LAN Servidores 172.8.63.128/28 | Server Web | 172.8.63.130 | |

---

## II. Imágenes en los dispositivos.

Aquí encontrara información de los componentes de la topología. Que fueron esenciales para poder comprobar y validar esta configuración con la cual contamos, para probar el funcionamiento del equipo Fortigate.

| Dispositivo | Nodo | Imagen |
|---|---|---|
| Fortigate | fortinet | Fortinet-FGT-7.0.9 |
| Switch | Cisco vIOS | Switch Viosl2-adventerprisek9-m.ssa.high_iron_20200929 |
| Linux PC | Docker.io | Pnetlab/linux-desktop:latest |
| DBServer | Docker.io | Pnetlab/mysql_server:latest |
| Web Server | Docker.io | Vulnerables/web-dvwa:latest |
