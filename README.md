# Infraestructura Avanzada para Automatización y Ciencia de Datos (n8n + JupyterLab)

Este repositorio contiene la arquitectura modular y segura diseñada para desplegar un entorno de automatización (*self-hosted*) y análisis de datos en producción utilizando Docker.

## 🚀 Desafíos Resueltos
1. **Persistencia de Datos:** Configuración de volúmenes locales para evitar la pérdida de flujos en n8n y scripts en JupyterLab al reiniciar contenedores.
2. **Seguridad y Webhooks:** Preparación del entorno para acoplar proxies inversos y certificados SSL (HTTPS), obligatorio para la integración con la API de Telegram.
3. **Inyección Segura de Credenciales:** Uso estricto de variables de entorno (`.env`) para aislar dominios y tokens de acceso.

## 🛠️ Stack Tecnológico
* **Orquestación:** Docker & Portainer.
* **Automatización:** n8n core.
* **Ciencia de Datos:** JupyterLab (DataScience Notebook con Python/SQL).

## 📸 Evidencia del Despliegue

### 0. Infraestructura Cloud (DigitalOcean Droplet)
<img width="1033" height="522" alt="consola" src="https://github.com/user-attachments/assets/2f56e1ac-24e4-4301-9d75-f0b89a39a584" />

### 1. Panel de Automatización (n8n)
<img width="1370" height="784" alt="n8n" src="https://github.com/user-attachments/assets/6fa13e80-605d-42d9-9872-62e904e370c7" />

### 2. Entorno de Ciencia de Datos (JupyterLab)
<img width="1374" height="789" alt="jupyterlab" src="https://github.com/user-attachments/assets/1b77f2f7-bda0-49e3-a6bf-2f5a5751165d" />
