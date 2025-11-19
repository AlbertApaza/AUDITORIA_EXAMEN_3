# Evidencia: Prueba de Funcionalidad del Sistema

**Fecha:** 19/11/2025  
**Auditor:** ALBERT KENYI APAZA CCALLE  

## Descripción
Se realizó una prueba completa del sistema levantado en Docker con el modelo smollm:360m.

1. **Acceso al frontend:** http://localhost:5173  
   - Interfaz carga correctamente.  
   - Chatbot responde a consultas generales (ej. "¿Qué es ACME?").  

2. **Generación de tickets:**  
   - Al enviar mensaje con problema, se genera ticket en base de datos.  
   - Confirmación de ticket recibido.  

3. **Procesamiento de lenguaje natural:**  
   - Respuestas basadas en documentos de knowledge_base.  
   - Modelo responde en español de forma concisa.  

**Resultado:** Sistema funcional al 100% según especificaciones.

## Capturas de Pantalla

### Interfaz del Chat
![Aquí va la imagen de la interfaz del chat](interfaz_chat.png)

### Ticket Generado
![Aquí va la imagen del ticket generado](ticket_generado.png)