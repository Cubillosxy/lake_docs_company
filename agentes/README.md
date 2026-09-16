# Memoria y Estado de Agentes de IA

Este directorio está destinado a funcionar como sistema de "State Management" (Gestión de Estado) y memoria para los diversos agentes de Inteligencia Artificial que operarán sobre este proyecto.

## Estructura de Información
Cada agente o proceso automatizado podrá leer y escribir en este directorio utilizando archivos Markdown o JSON para mantener contexto entre sesiones, guardar investigaciones, análisis de mercado y borradores de trabajo.

- **`contexto/`**: Para almacenar información profunda sobre la empresa.
- **`outputs/`**: Para guardar resultados de tareas delegadas a los agentes.
- **`logs/`**: Registro de decisiones y acciones tomadas por los agentes.
