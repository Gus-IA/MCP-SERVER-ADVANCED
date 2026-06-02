# 🚀 Model Context Protocol (MCP) – Advanced Topics

Este repositorio contiene un resumen y apuntes del curso **“Model Context Protocol: Advanced Topics”** impartido por Anthropic, disponible en Skilljar.

🔗 Curso original:  
https://anthropic.skilljar.com/model-context-protocol-advanced-topics

---

## 📚 Descripción del curso

Este curso explora los aspectos avanzados del **Model Context Protocol (MCP)**, un estándar diseñado para conectar modelos de lenguaje (LLMs) con herramientas, datos y sistemas externos de forma estructurada y segura.

A lo largo del curso se profundiza en cómo construir servidores MCP listos para producción, incluyendo patrones de comunicación, transporte de mensajes y funcionalidades avanzadas del protocolo.

---

## 🧠 Temas principales

### 🔹 Sampling
- Permite que los servidores MCP soliciten inferencias a modelos de lenguaje a través del cliente.
- Desacopla el coste y la ejecución del modelo del servidor.
- Facilita arquitecturas más seguras y escalables.

### 🔹 Notificaciones (Progress & Logging)
- Permiten enviar actualizaciones en tiempo real durante tareas largas.
- Mejoran la experiencia del usuario con feedback continuo.
- Incluyen logs y progreso de ejecución.

### 🔹 Roots
- Definen los puntos de acceso a archivos o directorios permitidos.
- Proporcionan control de permisos sobre el sistema de archivos.
- Permiten a los servidores trabajar sin conocer rutas exactas.

### 🔹 Tipos de mensajes JSON
- **Request / Result**: comunicación síncrona.
- **Notifications**: eventos sin respuesta.
- Base del intercambio de información en MCP.

### 🔹 Transportes

#### 🖥️ STDIO
- Comunicación local mediante entrada/salida estándar.
- Ideal para desarrollo y pruebas.

#### 🌐 StreamableHTTP
- Basado en HTTP + Server-Sent Events (SSE).
- Permite comunicación remota y streaming de eventos.
- Soporta escalabilidad y ejecución en producción.

---

## ⚙️ Inicialización MCP

El proceso de conexión sigue este flujo:

1. `Initialize Request`
2. `Initialize Result`
3. `Initialized Notification`

---

## 🔄 Casos de uso

- Integración de LLMs con sistemas externos
- Construcción de agentes inteligentes
- Automatización de flujos de trabajo
- Acceso controlado a archivos y recursos locales
- Arquitecturas distribuidas con IA

---

## 🏗️ Arquitectura MCP (resumen)

- Cliente ↔ Servidor mediante JSON-RPC
- Transporte por STDIO o HTTP
- Capas de seguridad mediante Roots
- Ejecución de herramientas externas
- Sampling para delegar inferencias al cliente

---

## 🎯 Aprendizajes clave

- MCP separa **modelo, herramientas y datos**
- Permite sistemas de IA más modulares y escalables
- Introduce un estándar para interoperabilidad entre LLMs y servicios
- Facilita el diseño de agentes avanzados

---

## 🧩 Tecnologías relacionadas

- Model Context Protocol (MCP)
- JSON-RPC
- Server-Sent Events (SSE)
- HTTP Streaming
- Arquitecturas de agentes IA

---

## 📌 Autor

Apuntes basados en el curso de Anthropic sobre MCP avanzado.

---

## 📄 Licencia

Uso educativo y personal.
