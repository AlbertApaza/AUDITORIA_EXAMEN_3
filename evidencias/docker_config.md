# Evidencia: Auditoría de Configuración Docker Compose

**Fecha:** 19/11/2025  
**Auditor:** ALBERT KENYI APAZA CCALLE  

## Análisis de docker-compose.yml

- **Servicios:** backend, frontend, proxy (nginx)  
- **Puertos expuestos:** 5173 (proxy)  
- **Volúmenes:** ./backend/vector_store para persistencia  
- **Extra hosts:** host.docker.internal para acceso a Ollama  
- **Dependencias:** frontend depende de backend, proxy de ambos  

## Hallazgos

- Puerto 5173 expuesto correctamente para acceso web.  
- Volúmenes aseguran persistencia de datos.  
- Configuración de red permite comunicación interna.  
- Ollama no está dockerizado, corre en host (puerto 11434).  

## Recomendación
Considerar dockerizar Ollama para mejor aislamiento.

## Archivo Adjunto
- docker-compose.yml  

## Capturas de Pantalla

### Configuración Docker
![Aquí va la imagen de la configuración Docker](docker_config.png)