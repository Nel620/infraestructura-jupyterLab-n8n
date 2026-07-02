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