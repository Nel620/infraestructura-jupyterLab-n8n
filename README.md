# 🧪 Infraestructura JupyterLab + n8n

Arquitectura modular en Docker para el despliegue integrado de n8n y JupyterLab,
optimizada para automatización de procesos y análisis de datos en entornos privados.

Proyecto desplegado en un servidor propio (DigitalOcean) con dominio, SSL y
proxy inverso.

## 📦 Stack Tecnológico

- **Docker & Docker Compose** — orquestación de contenedores
- **JupyterLab** (`jupyter/datascience-notebook`) — entorno de análisis de datos
- **n8n** — automatización de workflows
- **Nginx Proxy Manager** — reverse proxy + SSL automático (Let's Encrypt)
- **Portainer** — administración visual de contenedores

## 🧩 Desafíos Resueltos

- **Persistencia de datos:** volúmenes Docker para no perder notebooks ni workflows
- **SSL y proxy inverso:** configuración de Nginx Proxy Manager con Let's Encrypt
- **Webhooks seguros:** n8n expuesto vía HTTPS para integraciones externas
- **Debugging asistido:** uso de IA (Claude, Gemini, ChatGPT) como copiloto técnico para diagnosticar
  errores de despliegue (502, conectividad Docker, DNS) y documentar el proceso
  
## 📸 Evidencia del Despliegue

*(capturas existentes: droplet activo, n8n funcionando, JupyterLab funcionando)*

### 1. Servidor activo (DigitalOcean Droplet)
<img width="1033" height="522" alt="consola" src="https://github.com/user-attachments/assets/ee795e2c-2a40-429b-bbcb-e5a00e314a58" />

### 2. n8n en producción con SSL
<img width="1370" height="784" alt="n8n" src="https://github.com/user-attachments/assets/0afb05f9-04ef-44dd-9864-3c8984a94393" />

### 3. JupyterLab en producción con SSL
<img width="1374" height="789" alt="jupyterlab" src="https://github.com/user-attachments/assets/c0d26014-11c3-4a1b-ad98-6471d2a001b0" />

### 4. Certificado SSL válido (Nginx Proxy Manager)
<img width="1351" height="436" alt="proxy" src="https://github.com/user-attachments/assets/2e92b773-e0b7-4663-a34f-a6928ffefb2c" />
