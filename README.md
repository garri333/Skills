# 🧠 Skills — Librería de Skills para Agentes IA

[![Agent Skills Standard](https://img.shields.io/badge/Agent%20Skills-Standard-blue)](https://agentskills.io/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green)](LICENSE)
[![Skills: 220+](https://img.shields.io/badge/Skills-220%2B-orange)](skills/)

Repositorio de **220+ skills reutilizables para agentes IA** (GitHub Copilot, Claude Code, Cursor, Codex, Cline, Windsurf, etc.).

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
├── 01-writing-content/          # Escritura, copywriting, contenido, marketing
├── 02-frontend-design/          # UI/UX, React, diseño web, generación de imágenes
├── 03-backend-api/              # APIs, servidores, bases de datos
├── 04-ai-agents/                # Prompts, agentes, skills IA
├── 05-devops-git/               # Git, CI/CD, despliegues, MCP
├── 06-data-analysis/            # Datos, visualización, crypto, estadística
├── 07-security-compliance/      # Ciberseguridad, normativas
├── 08-automation/               # Email, calendario, tareas, búsqueda web
├── 09-research/                 # Investigación, análisis, DeepWiki, búsqueda
├── 10-privalex/                 # Skills específicas de PrivaLex Partners
├── 11-scientific/               # 117 skills científicas (K-Dense-AI)
├── 12-vercel-labs/              # 5 skills oficiales de Vercel Labs
├── 13-anthropic/                # 16 skills oficiales de Anthropic
├── 14-social-comms/             # Twitter/X, Slack, Discord, LinkedIn, Reddit
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
| `copywriting-persuasive` | Técnicas de copywriting persuasivo y conversión | Emails, ads, landing pages, sales copy |
| `humanizer` | Detecta y elimina marcadores de texto IA | Revisar textos antes de publicar |
| `marketing-mode` | 23 frameworks de marketing (AIDA, growth, CRO, SEO) | Estrategias de marketing y contenido |
| `prompt-log` | Extrae transcripts de sesiones de agentes | Documentar y revisar conversaciones IA |
| `resume-optimizer` | CV con scoring ATS y exportación PDF/DOCX | Crear o mejorar currículums |
| `seo-content` | Guía completa de SEO y estructura editorial | Crear blog posts, landing pages, contenido web |

### 02. Frontend y Diseño

| Skill | Descripción | Cuándo usar |
|-------|-------------|-------------|
| `frontend-design` | Guía de diseño UI/UX y accesibilidad | Revisar o crear interfaces web |
| `image-generation` | DALL-E 3, FLUX, Stable Diffusion — texto a imagen | Generar imágenes con IA |
| `react-best-practices` | Patrones React y Next.js de Vercel Engineering | Escribir o refactorizar código React |
| `react-composition-patterns` | Patrones de composición React escalables | Refactorizar componentes |
| `react-native-mobile` | React Native y Expo para apps móviles | Desarrollar apps móviles |
| `superdesign` | Expert guidelines para UIs modernas y hermosas | Crear interfaces premium |
| `uiux-pro` | Inteligencia de diseño UI/UX para interfaces pulidas | Proyectos con React, Vue, Svelte, Tailwind |
| `web-design-guidelines` | Guía de mejores prácticas para interfaces web | Auditar UI, accessibility, UX |

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
| `mcp-porter` | Descubrir, instalar y llamar servidores MCP | Gestionar el ecosistema MCP |
| `vercel-platform` | Deploy y gestión de proyectos en Vercel | Deployar, dominios, variables de entorno |

### 06. Datos y Análisis

| Skill | Descripción | Cuándo usar |
|-------|-------------|-------------|
| `crypto-wallet` | Wallets multi-chain: Ethereum, Polygon, Solana | Leer balances y transacciones blockchain |
| `data-visualization` | Crear visualizaciones de datos efectivas | Charts, gráficos, dashboards |
| `financial-analysis` | Análisis financiero de stocks y mercados | Finanzas, inversiones, mercados |
| `ga4-analytics` | Query Google Analytics 4 via API | Analizar métricas web |
| `statistical-analysis` | Análisis estadístico y metodología | Análisis de datos, informes |

### 07. Seguridad y Compliance

| Skill | Descripción | Cuándo usar |
|-------|-------------|-------------|
| `security-audit` | Auditoría de seguridad completa | Revisar configuraciones de seguridad |
| `security-monitor` | Monitorización de seguridad en tiempo real | Detectar intrusiones y anomalías |

### 08. Automatización

| Skill | Descripción | Cuándo usar |
|-------|-------------|-------------|
| `browser-automation` | Automatización de navegador (headless) | Scraping, testing, workflows web |
| `caldav-calendar` | Eventos de calendario via CalDAV (Google, iCloud) | Crear/leer eventos de calendario |
| `email` | Enviar/leer email via IMAP/SMTP y Gmail API | Notificaciones, automatización de email |
| `faster-whisper` | Transcripción de voz local con Whisper | Transcribir audio/video sin API |
| `google-workspace` | CLI para Gmail, Calendar, Drive, Contacts | Automatizar Google Workspace |
| `notion` | API de Notion — bases de datos, páginas, bloques | Gestión de conocimiento con Notion |
| `realtime-web-search` | Búsqueda web en tiempo real (Tavily, Serper, Brave) | Información actual y en tiempo real |
| `remind-me` | Crear recordatorios con lenguaje natural | Programar tareas futuras |
| `todoist` | Gestión de tareas via Todoist REST API | Crear y organizar tareas desde código |
| `weather` | Datos meteorológicos sin API key con wttr.in | Información del tiempo actual |
| `whatsapp-messaging` | Enviar mensajes WhatsApp via CLI | Notificaciones, mensajes automáticos |
| `youtube-downloader` | Descargar videos con yt-dlp | Descargar contenido de YouTube y más |

### 09. Research e Investigación

| Skill | Descripción | Cuándo usar |
|-------|-------------|-------------|
| `deepwiki` | Q&A sobre cualquier repositorio GitHub via DeepWiki | Entender librerías y codebases |
| `knowledge-base` | Sistema de gestión de conocimiento (LanceDB, RAG) | Gestionar knowledge base del proyecto |
| `research-deep` | Investigación profunda con arXiv, Semantic Scholar | Research complejo y papers científicos |
| `summarize-content` | Resumen inteligente de URLs o archivos | Leer y resumir contenido rápidamente |
| `thinking-partner` | Colaborador de pensamiento para problemas complejos | Explorar problemas con preguntas |
| `web-search-brave` | Búsqueda web via Brave Search API | Buscar documentación, hechos, noticias |
| `web-search-exa` | Búsqueda semántica con Exa AI | Encontrar código, papers, info empresa |

### 11. Scientific (K-Dense-AI — 117 skills)

> **Fuente:** [K-Dense-AI/claude-scientific-skills](https://github.com/K-Dense-AI/claude-scientific-skills)

Skills especializadas para investigación científica, bioinformática, química, física y ciencia de datos.

| Dominio | Skills destacadas |
|---------|-------------------|
| Bioinformática | scanpy, biopython, deeptools, pysam, pydeseq2, anndata, cellxgene-census |
| Química | rdkit, chembl-database, pubchem-database, matchms, molfeat, deepchem |
| Drug Discovery | drugbank-database, opentargets-database, diffdock, pytdc, medchem |
| Genómica | ensembl-database, gene-database, gwas-database, clinvar-database, gget |
| Clínica | pyhealth, clinical-reports, clinical-decision-support, clinpgx-database |
| Física / Quantum | qiskit, pennylane, cirq, qutip, fluidsim, pymatgen |
| ML / Datos | pytorch-lightning, polars, dask, networkx, plotly, matplotlib, pymc |
| Lab Automation | opentrons-integration, pylabrobot, lamindb, latchbio-integration |
| Publicación | latex-posters, pptx-posters, scientific-slides, paper-2-web, markitdown |
| Investigación | literature-review, hypothesis-generation, peer-review, scientific-brainstorming |

[→ Ver todas las 117 skills científicas](skills/11-scientific/)

### 12. Vercel Labs (Oficial — 5 skills)

> **Fuente:** [vercel-labs/agent-skills](https://github.com/vercel-labs/agent-skills)

| Skill | Descripción |
|-------|-------------|
| `composition-patterns` | Patrones avanzados de composición React |
| `react-best-practices` | Mejores prácticas React oficiales de Vercel |
| `react-native-skills` | Patrones oficiales de React Native |
| `vercel-deploy-claimable` | Deployments reclamables en Vercel |
| `web-design-guidelines` | Guías de diseño web oficiales de Vercel |

### 13. Anthropic (Oficial — 16 skills)

> **Fuente:** [anthropics/skills](https://github.com/anthropics/skills)

| Skill | Descripción |
|-------|-------------|
| `algorithmic-art` | Arte generativo y creative coding |
| `brand-guidelines` | Creación y aplicación de brand guidelines |
| `canvas-design` | Patrones de diseño para canvas/artifacts |
| `doc-coauthoring` | Escritura colaborativa de documentos |
| `docx` | Generación de documentos Word |
| `frontend-design` | Patrones de frontend de Anthropic |
| `internal-comms` | Escritura de comunicaciones internas |
| `mcp-builder` | Construir servidores MCP desde cero |
| `pdf` | Generación y manipulación de PDFs |
| `pptx` | Creación de presentaciones PowerPoint |
| `skill-creator` | Crear nuevas skills para agentes |
| `slack-gif-creator` | Creación de GIFs animados para Slack |
| `theme-factory` | Generación de temas de UI |
| `web-artifacts-builder` | Creación de artifacts web |
| `webapp-testing` | Testing de aplicaciones web |
| `xlsx` | Generación de hojas de cálculo Excel |

### 14. Social & Comunicaciones

| Skill | Descripción | Cuándo usar |
|-------|-------------|-------------|
| `bird-twitter` | X/Twitter — posts, búsqueda, timeline, DMs | Publicar o monitorear en X/Twitter |
| `discord` | Discord bots, webhooks, slash commands | Integrar con servidores Discord |
| `linkedin-cli` | LinkedIn — scraping de perfiles y automatización | Investigación de candidatos/empresas |
| `reddit` | Reddit lectura via JSON endpoints y PRAW | Monitorear hilos y subreddits |
| `slack` | Slack SDK, webhooks, file uploads, eventos | Notificaciones y bots de Slack |

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

| Categoría | Skills | Fuente |
|-----------|--------|--------|
| 01-10 Skills propias | 55 | Custom |
| 11 Científicas | 117 | K-Dense-AI |
| 12 Vercel Labs | 5 | Vercel Oficial |
| 13 Anthropic | 16 | Anthropic Oficial |
| 14 Social/Comms | 5 | Clawdbot-inspired |
| **Total** | **198+** | **Multi-fuente** |

- Categorías: 14
- Compatible con: GitHub Copilot, Claude Code, Cursor, Codex, Cline, Windsurf
- Fuentes: skills.sh, K-Dense-AI, Vercel Labs, Anthropic, clawdbotskills.org, Privalex custom

---

## 🤝 Créditos y Fuentes

- [K-Dense-AI/claude-scientific-skills](https://github.com/K-Dense-AI/claude-scientific-skills) — 117 skills científicas
- [vercel-labs/agent-skills](https://github.com/vercel-labs/agent-skills) — Skills oficiales de Vercel
- [anthropics/skills](https://github.com/anthropics/skills) — Skills oficiales de Anthropic
- [skills.sh](https://skills.sh) — Directorio de agent skills
- [clawdbotskills.org](https://clawdbotskills.org) — Marketplace de skills

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
