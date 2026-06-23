<h1 align = "center" >🌐 Iniciación al Subnetting con Cisco Packet Tracer</h1

[![Cisco](https://img.shields.io/badge/Cisco-1BA0D7?style=for-the-badge&logo=cisco&logoColor=white)](https://www.cisco.com/)
[![Packet Tracer](https://img.shields.io/badge/Packet%20Tracer-8.0+-blue?style=for-the-badge)](https://www.netacad.com/)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)
[![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)]()

## 📖 Descripción

Práctica de **subnetting** realizada con **Cisco Packet Tracer**. El proyecto incluye el cálculo completo de una dirección IP con notación CIDR /26, la creación de 4 subredes y la comprobación de conectividad entre equipos de la misma y diferente subred.

Diseñado como material educativo para estudiantes de **Sistemas Microinformáticos y Redes (SMR)**, aunque su contenido es aplicable a **ASIR** y a cualquier persona que quiera aprender los fundamentos del subnetting.

## 🎯 Objetivos del proyecto

- ✅ Calcular la máscara de red a partir de una notación CIDR (/26).
- ✅ Calcular la dirección de red, broadcast y rango de IPs.
- ✅ Calcular los bits de host y el número de hosts disponibles.
- ✅ Calcular el número de subredes posibles.
- ✅ Crear 4 subredes en Cisco Packet Tracer.
- ✅ Asignar direcciones IP a los equipos de cada subred.
- ✅ Comprobar la conectividad entre equipos de la misma subred.
- ✅ Comprobar la conectividad entre equipos de distinta subred.
- ✅ Comparar el comportamiento de un Hub vs un Switch.

## 📊 Cálculos realizados

### Datos de partida

- **IP:** 192.168.15.10/26
- **Notación CIDR:** /26

### Resultados

| **Concepto** | **Valor** |
|--------------|-----------|
| **Máscara de red** | 255.255.255.192 |
| **Dirección de red** | 192.168.15.0/26 |
| **Dirección de broadcast** | 192.168.15.63 |
| **Rango de IPs** | 192.168.15.1 - 192.168.15.62 |
| **Bits de host** | 6 |
| **Hosts disponibles** | 62 |
| **Subredes** | 4 |

### Subredes creadas

| **Subred** | **Red** | **Broadcast** | **Rango usable** |
|------------|---------|---------------|-------------------|
| **Subred 1** | 192.168.15.0/26 | 192.168.15.63 | 192.168.15.1 - 192.168.15.62 |
| **Subred 2** | 192.168.15.64/26 | 192.168.15.127 | 192.168.15.65 - 192.168.15.126 |
| **Subred 3** | 192.168.15.128/26 | 192.168.15.191 | 192.168.15.129 - 192.168.15.190 |
| **Subred 4** | 192.168.15.192/26 | 192.168.15.255 | 192.168.15.193 - 192.168.15.254 |

## 🛠️ Contenido del repositorio

| Archivo | Descripción |
|---------|-------------|
| `ARCONES HUGO PRACTICA CISCO PACKET TRACER SUBNETTING.pdf` | Manual completo con explicaciones, cálculos y capturas. |
| `subnetting.pkt` | Archivo de Packet Tracer con las 4 subredes configuradas. |

## 🚀 Cómo usar este proyecto

1. **Clona el repositorio**:
   ```bash
   git clone https://github.com/hugoarco/Packet-Tracer--Subnetting.git
Abre el archivo .pkt con Cisco Packet Tracer (versión 8.0 o superior).

Revisa las configuraciones:

Comprueba las IPs asignadas a cada PC.

Realiza pruebas de conectividad con ping.

Consulta el manual para entender el proceso paso a paso.


🔍 Pruebas de conectividad
Prueba	Origen	Destino	Resultado
Misma subred	PC1 (192.168.15.1)	PC2 (192.168.15.2)	✅ Éxito
Distinta subred	PC1 (192.168.15.1)	PC4 (192.168.15.65)	❌ Fallo

🧠 Comparativa Hub vs Switch
Dispositivo	Capa	Funcionamiento	Segmentación
Hub	Capa 1 (Física)	Repite señales a todos los puertos	❌ No segmenta
Switch	Capa 2 (Enlace)	Envía según dirección MAC	❌ No segmenta (necesita router)
Conclusión: Cambiar un Hub por un Switch NO afecta a la conectividad entre subredes, solo mejora el rendimiento interno de cada subred. Para conectar diferentes subredes se necesita un Router (Capa 3).

👤 Autor
Hugo Arco
Estudiante de SMR | Apasionado por la automatización, redes y administración de sistemas


📄 Licencia
Este proyecto está bajo la licencia MIT.
Consulta el archivo LICENSE para más información.

<p align="center"> <b>Hecho con ❤️, calculadora y mucho subnetting</b> </p> ```
