# 🧠 Memoria y Estado de Agentes de IA

Este directorio está destinado a funcionar como sistema de "State Management" (Gestión de Estado) y memoria para los diversos agentes de Inteligencia Artificial que operarán sobre este proyecto.

## 📂 Estructura de Información
Cada agente o proceso automatizado podrá leer y escribir en este directorio utilizando archivos Markdown o JSON para mantener contexto entre sesiones, guardar investigaciones, análisis de mercado y borradores de trabajo.

- **`contexto/`**: Para almacenar información profunda sobre la empresa.
- **`outputs/`**: Para guardar resultados de tareas delegadas a los agentes.
- **`logs/`**: Registro de decisiones y acciones tomadas por los agentes.

---

## 🤝 Guía de Colaboración (Para Humanos y Agentes)

Este proyecto está diseñado para que múltiples desarrolladores, colaboradores y agentes de IA puedan trabajar de forma asíncrona. Sigue estas reglas estrictas para mantener el orden y la funcionalidad del Dashboard:

### 1. Regla de "Single Page" (No crear nuevos tabs/páginas)
Para mantener la compatibilidad fluida con nuestra configuración actual de **GitHub Pages**, **NO se deben crear nuevas páginas HTML o Markdown separadas para la navegación principal**. 
- Todo el contenido nuevo que deba ser visible públicamente en el Dashboard debe agregarse como **nuevas secciones** (con subtítulos `##`) dentro del archivo principal `index.md`.
- Puedes crear hipervínculos internos (anclas como `[Enlace](#mi-nueva-seccion)`) para saltar a esas partes.
- El directorio `agentes/` es estrictamente para almacenamiento de datos (JSON, MD en crudo) y memoria en segundo plano, no para generar vistas públicas.

### 2. ¿Cómo colaborar y proponer cambios? (Fork & PR)
Para proponer cambios, mejorar la planeación, o dejar que otros agentes realicen tareas de manera paralela sin dañar la versión oficial (producción), utiliza el flujo estándar de Git:

1. **Haz un Fork (Bifurcación):** Ve al repositorio oficial en GitHub y haz clic en el botón `Fork` (esquina superior derecha). Esto creará una copia del repositorio en tu propia cuenta.
2. **Clona tu Fork localmente:**
   ```bash
   git clone https://github.com/TU_USUARIO/lake_docs_company.git
   cd lake_docs_company
   ```
3. **Crea una nueva rama (Branch):** Crea una rama específica para la mejora, investigación o tarea que vayas a realizar:
   ```bash
   git checkout -b feature/mejora-analisis-mercado
   ```
4. **Trabaja y actualiza la memoria:** Realiza los cambios. Si estás ejecutando agentes de IA, asegúrate de que sus procesos guarden el estado en las subcarpetas de `agentes/`.
5. **Guarda y sube tus cambios (Commit & Push):**
   ```bash
   git add .
   git commit -m "feat: Agregado análisis de competencia al dashboard"
   git push origin feature/mejora-analisis-mercado
   ```
6. **Envía un Pull Request (PR):** Ve a la página de tu repositorio en GitHub y aparecerá un botón verde que dice `Compare & pull request`. Añade una buena descripción de lo que tú (o tus agentes) hicieron. El dueño del proyecto revisará tu solicitud y la integrará (Merge) a la base principal.
