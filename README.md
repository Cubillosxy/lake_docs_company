# Dashboard y Memoria de Proyecto: Empresa AI y Marketing

Este repositorio funciona como el **Panel de Control (Dashboard)** y el sistema de **Gestión de Estado (State Management)** para la planificación e implementación de nuestra nueva empresa de Inteligencia Artificial y Marketing en Colombia.

El propósito de este proyecto no es alojar el código fuente de los productos finales, sino centralizar la planificación estratégica (fases, tareas, objetivos) y proveer un entorno de memoria para que diversos agentes de Inteligencia Artificial puedan colaborar y persistir su contexto.

## Estructura del Repositorio

- `index.md`: Panel de control principal. Toda la planeación (fases, objetivos, tareas) vive aquí como secciones, siguiendo la regla de "Single Page" para mantener compatibilidad con GitHub Pages.
- `agentes/`: Directorio destinado a la memoria y almacenamiento de contexto para los agentes de IA.
  - `agentes/contexto/`: Información profunda sobre la empresa.
  - `agentes/outputs/`: Resultados de tareas delegadas a los agentes.
  - `agentes/logs/`: Registro de decisiones y acciones tomadas por los agentes.

## ¿Cómo visualizar el sitio?

Este repositorio está configurado para desplegarse fácilmente usando **GitHub Pages**. 
Una vez desplegado en GitHub, podrás acceder al Dashboard mediante la URL generada por GitHub Pages.

## ¿Cómo rodar el Dashboard localmente?

Si deseas previsualizar los cambios en tu computadora antes de subirlos a GitHub, puedes levantar el sitio localmente usando Jekyll (el generador de sitios estáticos que usa GitHub Pages por defecto).

### Requisitos previos
Necesitas tener instalado en tu sistema operativo:
- **Ruby** y **RubyGems**
- **Bundler** (puedes instalarlo ejecutando `gem install bundler`)

### Pasos para ejecución local

1. **Clona el repositorio** y navega hasta la carpeta del proyecto:
```bash
   git clone <url-del-repositorio>
   cd lake_docs_company
```

2. **Crea un archivo Gemfile** (si no existe) para instalar Jekyll y las dependencias de GitHub Pages. Puedes crear un archivo llamado `Gemfile` en la raíz con este contenido:
```ruby
   source "https://rubygems.org"
   gem "github-pages", group: :jekyll_plugins
```

3. **Instala las dependencias**:
```bash
   bundle install
```

4. **Levanta el servidor local**:
```bash
   bundle exec jekyll serve
```

5. **Visualiza el sitio**:
   Abre tu navegador web y visita: `http://localhost:4000`

Cualquier cambio que realices en los archivos `.md` se actualizará automáticamente en tu navegador al recargar la página.