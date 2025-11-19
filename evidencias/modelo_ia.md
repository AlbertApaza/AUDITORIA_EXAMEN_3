# Evidencia: Evaluación del Modelo de IA smollm:360m

**Fecha:** 19/11/2025  
**Auditor:** ALBERT KENYI APAZA CCALLE  

## Modelo Utilizado
- **Modelo:** smollm:360m  
- **Plataforma:** Ollama  

## Análisis
- Modelo lightweight adecuado para inferencia local.  
- Integración correcta con backend via http://host.docker.internal:11434  
- Respuestas en español, concisas y útiles.  
- Procesamiento RAG con Chroma para contexto relevante.  
- Rendimiento: Respuestas en <5 segundos en hardware estándar.  

## Pruebas Realizadas
1. **Consulta general:** "¿Cómo configurar red?" -> Respuesta basada en guia_soporte_red.pdf  
2. **Reporte de problema:** "No funciona el sistema" -> Genera ticket y sugiere solución.  
3. **Despedida:** "Gracias" -> Respuesta cortés.  

## Conclusión
Modelo adecuado para el propósito, buen balance entre tamaño y capacidad.

## Capturas de Pantalla

### Respuesta del Modelo
![Aquí va la imagen de respuesta del modelo IA](respuesta_modelo.png)