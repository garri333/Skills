# 🧠 Skills — Librería de Skills para Agentes IA

[![Agent Skills Standard](https://img.shields.io/badge/Agent%20Skills-Standard-blue)](https://agentskills.io/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green)](LICENSE)

Repositorio de **skills reutilizables para agentes IA** (GitHub Copilot, Claude Code, Cursor, Codex, etc.).

Cada skill es un conjunto de conocimiento especializado que el agente detecta automáticamente y aplica cuando es relevante para la tarea.

---

## 🎯 Para qué sirve este repositorio

Cuando empiezas un proyecto nuevo, el agente puede buscar en este repo y encontrar las skills que necesita:
- **¿Estás haciendo una web?** → Carga `frontend-design`, `web-design-guidelines`, `seo-content`
- **¿Estás haciendo un agente IA?** → Carga `prompt-engineering`, `memory-management`, `skill-creator`
- **¿Estás haciendo una API?** → Carga `api-design`, `git-conventional-commits`, `testing-strategy`
- **¿Necesitas contenido?** → Carga las skills de PrivaLex (`privalex-voice-and-tone`, etc.)

---

## 📦 Estructura del repositorio

```
skills/
├── 01-writing-content/          # Escritura, copywriting, contenido
├── 02-frontend-design/          # UI/UX, React, CSS, diseño web
├── 03-backend-api/              # APIs, servidores, bases de datos
├── 04-ai-agents/                # Prompts, agentes, skills IA
├── 05-devops-git/               # Git, CI/CD, despliegues
├── 06-data-analysis/            # Datos, visualización, estadística
├── 07-security-compliance/      # Ciberseguridad, normativas
├── 08-automation/               # Automatización, scripting,
├── 09-research/                 # Investigación, análisis, búsqueda
├── 10-privalex/                 # Skills específicas de PrivaLex Partners
└── _templates/                  # Plantillas para crear nuevas skills
```

---

## 🚀 Cómo usar este repositorio

### Opción 1: Instalación global (recomendado)
Las skills están disponibles en todos tus proyectos:

```bash
# Para Cursor
cp -r skills/* ~/.cursor/skills/

# Para Claude Code
cp -r skills/* ~/.claude/skills/

# Para Codex
cp -r skills/* ~/.codex/skills/
```

### Opción 2: Instalación por proyecto
Copia solo las skills que necesitas en tu proyecto:

```bash
mkdir -p .cursor/skills
cp -r skills/04-ai-agents/prompt-engineering .cursor/skills/
cp -r skills/02-frontend-design/frontend-design .cursor/skills/
```

### Opción 3: Usando npx (skills.sh ecosystem)
```bash
npx skills add garri333/skills/prompt-engineering
npx skills add garri333/skills/frontend-design
```

---

## 📋 Catálogo de Skills

### 01. Escritura y Contenido

| Skill | Descripción | Cuándo usar |
|-------|-------------|-------------|
| `seo-content` | Guía completa de SEO y estructura editorial | Crear blog posts, landing pages, contenido web |
| `copywriting-persuasive` | Técnicas de copywriting persuasivo y conversión | Emails, ads, landing pages, sales copy |
| `humanizer` | Detecta y elimina marcadores de texto IA | Revisar textos antes de publicar |
| `prompt-log` | Extrae transcripts de sesiones de agentes | Documentar y revisar conversaciones IA |

### 02. Frontend y Diseño

| Skill | Descripción | Cuándo usar |
|-------|-------------|-------------|
| `frontend-design` | Guía de diseño UI/UX y accesibilidad | Revisar o crear interfaces web |
| `react-best-practices` | Patrones React y Next.js de Vercel Engineering | Escribir o refactorizar código React |
| `web-design-guidelines` | Guía de mejores prácticas para interfaces web | Auditar UI, accessibility, UX |
| `react-composition-patterns` | Patrones de composición React escalables | Refactorizar componentes |
| `react-native-mobile` | React Native y Expo para apps móviles | Desarrollar apps móviles |
| `superdesign` | Expert guidelines para UIs modernas y hermosas | Crear interfaces premium |
| `uiux-pro` | Inteligencia de diseño UI/UX para interfaces pulidas | Proyectos con React, Vue, Svelte, Tailwind |

### 03. Backend y APIs

| Skill | Descripción | Cuándo usar |
|-------|-------------|-------------|
| `api-design` | Principios y patrones para diseñar APIs robustas | Diseñar o revisar APIs REST/GraphQL |
| `vercel-deploy` | Despliegue de aplicaciones en Vercel | Deployar apps web |
| `excel-data` | Leer, escribir y manipular archivos Excel | Trabajar con datos en Excel |
| `pdf-builder` | Generar PDFs profesionales desde Markdown | Crear documentos, reports, NDAs |

### 04. Agentes IA

| Skill | Descripción | Cuándo usar |
|-------|-------------|-------------|
| `prompt-engineering` | Técnicas avanzadas de ingeniería de prompts | Crear o mejorar prompts |
| `skill-creator` | Guía para crear nuevas skills | Crear una skill nueva |
| `memory-management` | Configurar memoria persistente para agentes | Añadir memoria a un agente |
| `self-improving-agent` | Captura aprendizajes para mejorar performance | Agentes que aprenden de sus errores |
| `deep-research-agent` | Investigación compleja multi-step | Tareas de investigación profunda |
| `coding-agent` | Control de agentes de coding (Claude Code, Codex) | Programar mediante subagentes |

### 05. DevOps y Git

| Skill | Descripción | Cuándo usar |
|-------|-------------|-------------|
| `git-conventional-commits` | Formato Conventional Commits para mensajes git | Hacer commits, changelogs, versionado |
| `github-cli` | Interfaz especializada con GitHub CLI (`gh`) | Issues, PRs, CI/CD, GitHub API |
| `vercel-platform` | Deploy y gestión de proyectos en Vercel | Deployar, dominios, variables de entorno |

### 06. Datos y Análisis

| Skill | Descripción | Cuándo usar |
|-------|-------------|-------------|
| `data-visualization` | Crear visualizaciones de datos efectivas | Charts, gráficos, dashboards |
| `statistical-analysis` | Análisis estadístico y metodología | Análisis de datos, informes |
| `ga4-analytics` | Query Google Analytics 4 via API | Analizar métricas web |
| `financial-analysis` | Análisis financiero de stocks y mercados | Finanzas, inversiones, mercados |

### 07. Seguridad y Compliance

| Skill | Descripción | Cuándo usar |
|-------|-------------|-------------|
| `security-audit` | Auditoría de seguridad completa | Revisar configuraciones de seguridad |
| `security-monitor` | Monitorización de seguridad en tiempo real | Detectar intrusiones y anomalías |

### 08. Automatización

| Skill | Descripción | Cuándo usar |
|-------|-------------|-------------|
| `browser-automation` | Automatización de navegador (headless) | Scraping, testing, workflows web |
| `remind-me` | Crear recordatorios con lenguaje natural | Programar tareas futuras |
| `google-workspace` | CLI para Gmail, Calendar, Drive, Contacts | Automatizar Google Workspace |
| `whatsapp-messaging` | Enviar mensajes WhatsApp via CLI | Notificaciones, mensajes automáticos |
| `youtube-downloader` | Descargar videos con yt-dlp | Descargar contenido de YouTube y más |

### 09. Research e Investigación

| Skill | Descripción | Cuándo usar |
|-------|-------------|-------------|
| `web-search-brave` | Búsqueda web via Brave Search API | Buscar documentación, hechos, noticias |
| `web-search-exa` | Búsqueda semántica con Exa AI | Encontrar código, papers, info empresa |
| `research-deep` | Investigación profunda con Gemini CLI | Research complejo sin quemar tokens Claude |
| `summarize-content` | Resumen inteligente de URLs o archivos | Leer y resumir contenido rápidamente |
| `knowledge-base` | Sistema de gestión de conocimiento (ByteRover) | Gestionar knowledge base del proyecto |
| `thinking-partner` | Colaborador de pensamiento para problemas complejos | Explorar problemas con preguntas |

### 10. PrivaLex Partners

| Skill | Descripción | Cuándo usar |
|-------|-------------|-------------|
| `privalex-product` | Positioning, servicios y proof points de PrivaLex | Cualquier contenido que describe PrivaLex |
| `privalex-voice-and-tone` | Voz, tono y guardarraíles anti-fluff | TODO el contenido de PrivaLex |
| `compliance-frameworks` | Base de conocimiento: ISO 27001, NIS2, GDPR, etc. | Contenido técnico de compliance |
| `seo-guidelines` | SEO específico para contenido PrivaLex | Blog posts y contenido web |
| `target-personas` | Perfiles de CISO, CTO, DPO, Founder | Personalizar contenido por audiencia |
| `content-formats` | Templates: blog, LinkedIn, newsletter, case study | Generar formatos específicos |
| `competitive-landscape` | Posicionamiento vs Vanta, ECIJA, etc. | Contenido comparativo |
| `examples-hall-of-fame` | Ejemplos aprobados de contenido PrivaLex | Referencia de calidad y tono |

---

## 🛠️ Cómo crear una nueva skill

Ver plantilla en [`_templates/SKILL-TEMPLATE.md`](_templates/SKILL-TEMPLATE.md)

Estructura básica:
```
skills/
└── mi-skill/
    ├── SKILL.md        ← OBLIGATORIO: Descripción + conocimiento
    └── examples/       ← OPCIONAL: Ejemplos de uso
        └── example-01.md
```

El `SKILL.md` debe empezar con frontmatter YAML:
```yaml
---
name: mi-skill
version: 1.0.0
description: Breve descripción de una línea. Cuándo el agente debe usarla.
tags: [categoria, herramienta, lenguaje]
author: garri333
license: MIT
---
```

---

## 📊 Estadísticas

- Total skills: 40+
- Categorías: 10
- Fuentes: skills.sh, clawdbotskills.org, K-Dense Scientific, PrivaLex custom
- Compatible con: GitHub Copilot, Claude Code, Cursor, Codex, Cline, Windsurf

---

## 🤝 Contribuir

1. Fork el repositorio
2. Crea tu skill siguiendo la plantilla en `_templates/`
3. Añádela en la categoría correcta
4. Actualiza este README
5. Pull Request

---

## 📝 Licencia

MIT — Libre para usar, modificar y distribuir.

Skills individuales pueden tener sus propias licencias (ver frontmatter de cada `SKILL.md`).

---

*Skills ecosystem powered by [skills.sh](https://skills.sh/) · Compatible con el [Agent Skills Standard](https://agentskills.io/)*
