# Eldritch – Agente de Inteligencia Artificial

## Pre-entrega 3 | AI Automation

### Descripción del proyecto

Eldritch es un agente de inteligencia artificial desarrollado mediante n8n y OpenAI, diseñado para recibir solicitudes a través de un Webhook, procesarlas mediante un modelo de lenguaje y ejecutar acciones automatizadas.

El proyecto integra inteligencia artificial, memoria conversacional, Gmail, Slack y lógica condicional.

### Tecnologías utilizadas

- **n8n:** automatización y orquestación de flujos.
- **OpenAI:** procesamiento de lenguaje natural.
- **Webhook:** recepción de solicitudes HTTP.
- **Gmail:** envío automatizado de correos electrónicos.
- **Slack:** envío de notificaciones.
- **GitHub:** documentación y control de versiones.

### Funcionamiento del flujo

1. El Webhook recibe una solicitud HTTP POST.
2. El agente de IA interpreta el mensaje recibido.
3. El modelo de OpenAI genera una respuesta.
4. La memoria simple permite mantener contexto conversacional.
5. Un nodo IF evalúa si el mensaje contiene la palabra "URGENTE".
6. Según el resultado, el flujo dirige la notificación a una de dos ramas de Slack.
7. El agente también dispone de herramientas para enviar mensajes mediante Gmail y Slack.

### Pruebas realizadas

- Recepción de solicitudes HTTP mediante Postman.
- Respuestas del Webhook con estado HTTP 200 OK.
- Ejecución exitosa del agente de IA.
- Validación de la condición URGENTE.
- Envío exitoso de mensajes a Slack.
- Envío exitoso de un correo electrónico mediante Gmail.

### Archivos del repositorio

- `checkpoint1.json`: primer checkpoint del proyecto.
- `checkpoint2.json`: segundo checkpoint del proyecto.
- `Eldritch_Preentrega3_GitHub.json`: exportación del flujo de la Pre-entrega 3.

### Resultado

Se desarrolló y probó un flujo de automatización que integra inteligencia artificial con servicios de comunicación y lógica de decisión, permitiendo procesar solicitudes y ejecutar acciones según las condiciones configuradas.

### Consideraciones de seguridad

Las credenciales y claves privadas no deben incluirse en los archivos exportados al repositorio. Para ejecutar el flujo en otra instancia de n8n, es necesario configurar las credenciales correspondientes.
