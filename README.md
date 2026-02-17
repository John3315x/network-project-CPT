# 📡 Proyecto de Infraestructura de Red – Cisco Packet Tracer

## 📌 Objetivo del proyecto

Este proyecto simula una infraestructura de red corporativa distribuida en varias sedes, con el objetivo de practicar diseño jerárquico, segmentación de red, servicios internos y control de acceso, utilizando Cisco Packet Tracer como entorno de laboratorio.

El enfoque principal es construir una red funcional, segura y realista, similar a la utilizada en empresas.

---

## 🌍 Topología de red

La red está distribuida en tres ubicaciones principales:

### Londres
- Servidor central (HTTP y DNS)  
- Conexión directa al ISP simulado  

### Bristol
- Área de infraestructura y varios departamentos  
- Segmentación mediante VLANs  
- Conexión al ISP simulado  
- Acceso controlado según políticas de red 
- Wifi de invitados 
- Enlace hacia Gloucester  

### Gloucester
- Hotel conectado a la red de Bristol  
- Wifi para clientes

El diseño sigue una estructura jerárquica (core, distribución y acceso).

---

## ⚙️ Servicios implementados

- VLANs para segmentación por departamentos y usuarios  
- DHCP para asignación automática de direcciones IP  
- NAT para salida a Internet desde redes internas  
- ACLs estándar y extendidas para control de tráfico  
- Servidor HTTP para pruebas de conectividad  
- DNS (en desarrollo)  
- Firewall y políticas de seguridad (en desarrollo)   

---

## 🧪 Cómo probar el proyecto

1. Abrir el archivo `.pkt` en **Cisco Packet Tracer**  
2. Verificar asignación de IP por DHCP en los dispositivos  
3. Probar conectividad:
   ```bash
   ping 172.26.17.3

