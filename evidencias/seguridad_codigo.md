# Evidencia: Análisis de Seguridad del Código

**Fecha:** 19/11/2025  
**Auditor:** ALBERT KENYI APAZA CCALLE  

## Análisis de backend/main.py

### Hallazgos de Seguridad
1. **Falta de autenticación:** Endpoint /ask sin auth (línea 111).  
2. **CORS permite "*":** allow_origins=["*"] (línea 47).  
3. **Exposición de Ollama:** Acceso directo a host.docker.internal:11434.  
4. **Logs incluyen datos sensibles:** Sin sanitización (línea 141).  
5. **Dependencias vulnerables:** langchain versiones antiguas.  

### Riesgos
- Acceso no autorizado a API.  
- Posible inyección o abuso del modelo IA.  
- Fuga de información en logs.  

### Recomendaciones
- Implementar JWT auth.  
- Restringir CORS a dominios específicos.  
- Configurar firewall para Ollama.  
- Sanitizar logs.  
- Actualizar dependencias.  

## Archivo Adjunto
- main.py (extractos relevantes)  

## Capturas de Pantalla

### Código Vulnerable
![Aquí va la imagen del código vulnerable](codigo_vulnerable.png)

### Logs Sensibles
![Aquí va la imagen de logs con datos sensibles](logs_sensibles.png)