# Prompts de Infografia — Synapis + Hermes: Domina tus dos agentes AI

> Diseñados como **experto pedagogico en mapas visuales y flujo de datos**.
> Cada prompt genera una infografia que facilita la comprension visual del concepto.
> Estilo consistente: dark mode (#0a0a14), glassmorphism, teal (Synapis) + purple (Hermes) + amber (bridge).

---

## Leccion 1: Que es un agente AI y por que necesitas dos
**Tipo de visualizacion**: Mind map con nodo central + 2 ramas principales

```
PROMPT — Plataforma: Canva / Figma

Crea un mind map educativo sobre fondo oscuro (#0a0a14) con bordes glassmorphism.

NODO CENTRAL: "Agentes AI" — circulo grande color amber (#f59e0b) con icono de cerebro+engranaje.

RAMA IZQUIERDA (color teal #0d9488, etiqueta "SYNAPIS"):
- Nodo: "Cerebro adaptativo" con sub-nodos:
  - "Observa como trabajas" (icono ojo)
  - "Aprende patrones" (icono grafo)
  - "Evoluciona skills" (icono flecha circular)
  - "Vive DENTRO de Claude Code" (icono caja contenedora)

RAMA DERECHA (color purple #7c3aed, etiqueta "HERMES"):
- Nodo: "Cuerpo autonomo" con sub-nodos:
  - "Ejecuta en terminal" (icono terminal)
  - "Multi-modelo (15+ providers)" (icono red de nodos)
  - "Gateway: Telegram, Discord..." (icono mensajes)
  - "Cron: tareas automaticas" (icono reloj)

CONEXION CENTRAL (linea amber punteada entre ambas ramas):
- Etiqueta: "Complementarios, NO competidores"
- Sub-etiqueta: "El cerebro sin el cuerpo solo piensa. El cuerpo sin el cerebro no sabe que hacer."

Tipografia: Space Mono para etiquetas tecnicas, Outfit para titulos.
Sin emojis reales — usar iconos minimalistas line-art.
Formato: 1920x1080px horizontal.
```

---

## Leccion 2: Synapis — instalar tu copiloto de desarrollo
**Tipo de visualizacion**: Diagrama de flujo vertical (instalacion paso a paso)

```
PROMPT — Plataforma: Figma

Crea un diagrama de flujo vertical de instalacion sobre fondo oscuro (#0a0a14).

TITULO: "Instalar Synapis en 4 pasos" — teal (#0d9488)

PASO 1 (caja redondeada teal):
  Input: "git clone https://github.com/Luispitik/synapis"
  Icono: carpeta con flecha
  Nota al lado: "Descarga el codigo fuente"

FLECHA DESCENDENTE (teal, con label "→")

PASO 2 (caja redondeada teal):
  Input: "./install.sh (Linux/Mac) | install.bat (Windows)"
  Icono: engranaje
  Nota al lado: "Copia skills a ~/.claude/skills/"

FLECHA DESCENDENTE

PASO 3 (caja redondeada teal):
  Input: "Claude Code lee CLAUDE.md al iniciar"
  Icono: documento con rayo
  Nota al lado: "Bootstrap automatico — Synapis se activa solo"

FLECHA DESCENDENTE

PASO 4 (caja redondeada amber, mas grande):
  Input: "_operator-state.json creado"
  Icono: persona con engranaje
  Nota: "Tu perfil: nombre, rol, stack, preferencias"
  Sub-nota: "Se carga ANTES de cada sesion"

A LA DERECHA del flujo, caja glassmorphism con titulo "Que se instala":
  - ~/.claude/CLAUDE.md (entry point)
  - ~/.claude/skills/ (5 skills globales)
  - ~/.claude/skills/_library/ (skills dormantes)
  - ~/.claude/skills/_catalog.json (registro)
  - ~/.claude/skills/_operator-state.json (tu perfil)

Formato: 1080x1920px vertical (ideal para stories/movil).
```

---

## Leccion 3: Tu primera sesion con Synapis
**Tipo de visualizacion**: Diagrama de secuencia (actor → sistema → resultado)

```
PROMPT — Plataforma: Figma

Crea un diagrama de secuencia UML simplificado sobre fondo oscuro.

ACTORES (3 columnas):
  - TU (icono persona, color blanco)
  - SYNAPIS (icono cerebro, color teal #0d9488)
  - CLAUDE CODE (icono terminal, color azul #4a9eed)

SECUENCIA:

1. TU → CLAUDE CODE: "Abres Claude Code en tu proyecto"
   CLAUDE CODE → SYNAPIS: "Lee CLAUDE.md → carga operator-state"
   SYNAPIS → CLAUDE CODE: "Inyecta skills globales en contexto"

2. SYNAPIS → TU: "Presenta opciones: [1] Skills on Demand [2] Skill Picker [3] Freestyle"
   TU → SYNAPIS: "Elige [1] Skills on Demand"

3. TU → CLAUDE CODE: "Trabajas normalmente: editas codigo, pides ayuda"
   SYNAPIS (caja sombreada teal): "OBSERVA EN SILENCIO"
   - Registra: correcciones que haces
   - Registra: preferencias de formato
   - Registra: tool chains repetidas
   Flecha punteada a: "_observations.json"

4. SYNAPIS → TU (notificacion sutil): "Detectados 3 patrones en esta sesion"

Estilo: lineas rectas, flechas con punta, cajas redondeadas.
Fondo: #0a0a14 con grid sutil.
Formato: 1920x1080px horizontal.
```

---

## Leccion 4: Hermes — instalar tu agente personal
**Tipo de visualizacion**: Diagrama de flujo con decision (branching por OS)

```
PROMPT — Plataforma: Figma

Crea un diagrama de flujo de instalacion con decision branch por sistema operativo.
Fondo oscuro (#0a0a14), color principal purple (#7c3aed).

INICIO (circulo): "Instalar Hermes Agent"

DECISION (diamante): "Que sistema operativo?"
  - Rama izquierda: "Linux / Mac" → "curl installer | bash"
  - Rama central: "Windows + Git Bash" → "Clone manual + venv + pip install"
  - Rama derecha: "Windows PowerShell" → "irm install.ps1 | iex"

Las 3 ramas CONVERGEN en:

PASO COMUN 1 (caja purple):
  "Editar config.yaml"
  Codigo: provider: "anthropic" | default: "claude-sonnet-4"

PASO COMUN 2 (caja purple):
  "Editar .env"
  Codigo: ANTHROPIC_API_KEY=tu-clave-aqui

PASO COMUN 3 (caja amber):
  "hermes doctor → todo verde"
  Checklist visual: Python ✓, Packages ✓, Config ✓, Directories ✓

RESULTADO FINAL (caja grande purple con glow):
  "hermes chat → tu agente personal responde"

A la derecha, caja glassmorphism "Donde vive todo":
  - %LOCALAPPDATA%\hermes\config.yaml
  - %LOCALAPPDATA%\hermes\.env
  - %LOCALAPPDATA%\hermes\memories/
  - %LOCALAPPDATA%\hermes\sessions/
  - %LOCALAPPDATA%\hermes\skills/

Formato: 1920x1080px horizontal.
```

---

## Leccion 5: Hermes — comandos esenciales
**Tipo de visualizacion**: Cheatsheet / referencia rapida en grid

```
PROMPT — Plataforma: Canva

Crea un cheatsheet de referencia rapida estilo "dark terminal" sobre fondo #0a0a14.

TITULO: "Hermes Agent — Comandos Esenciales" (purple #7c3aed)

GRID 3x4 de cards con bordes glassmorphism:

Card 1 (purple): hermes chat
  "Chat interactivo con el agente"
  Icono: burbuja de dialogo

Card 2 (purple): hermes model
  "Cambiar modelo/provider"
  Icono: switch/toggle

Card 3 (purple): hermes status
  "Ver config, API keys, gateway"
  Icono: dashboard

Card 4 (purple): hermes doctor
  "Diagnostico completo"
  Icono: estetoscopio

Card 5 (purple): hermes --continue
  "Retomar ultima sesion"
  Icono: play/resume

Card 6 (purple): hermes sessions list
  "Ver conversaciones pasadas"
  Icono: lista/historial

Card 7 (purple): hermes tools
  "Activar/desactivar tools"
  Icono: caja de herramientas

Card 8 (purple): hermes cron
  "Tareas automaticas"
  Icono: reloj

Card 9 (purple): hermes gateway start
  "Activar bot Telegram/Discord"
  Icono: antena/broadcast

Card 10 (amber): hermes config set
  "Cambiar config sin editar archivos"
  Icono: llave inglesa

Card 11 (amber): hermes skills
  "Marketplace de skills"
  Icono: tienda

Card 12 (amber): hermes update
  "Actualizar a ultima version"
  Icono: flecha circular

Seccion inferior: "Slash commands en chat"
  /new | /retry | /compress | /model | /save | /usage
  En fuente monospace sobre fondo ligeramente mas claro.

Formato: 1920x1080px horizontal. Ideal para wallpaper de escritorio.
```

---

## Leccion 6: Synapis a fondo — observacion, scoring y evolucion
**Tipo de visualizacion**: Diagrama de flujo de datos (data flow) multi-nivel

```
PROMPT — Plataforma: Figma

Crea un diagrama de flujo de datos complejo sobre fondo oscuro (#0a0a14).
Este es el diagrama mas tecnico del curso — nivel avanzado.

SECCION SUPERIOR — "Motor de Observacion" (teal)
  6 entradas paralelas (cajas pequeñas teal):
    [Correcciones] [Repeticiones] [Preferencias]
    [Workarounds] [Tool Chains] [Rechazos]
  Todas las flechas convergen en:
    → caja grande: "synapis-learning (observer)"
    → output: "_observations.json"

SECCION MEDIA — "Scoring Lifecycle" (teal → amber gradiente)
  Barra horizontal de progreso con 5 etapas:
    [Observation 0.0-0.3] → [Hypothesis 0.3-0.5] → [Pattern 0.5-0.7] → [Instinct 0.7-0.9] → [Law 0.9-1.0]
  Cada etapa con color progresivo de teal claro a teal oscuro.
  Flecha descendente con label "-0.05 cada 30 dias" (decay, color rojo sutil)
  Flecha descendente con label "< 0.20 → excluido del prompt" (rojo)

SECCION INFERIOR — "Pipeline /evolve" (amber #f59e0b)
  Input: "Instincts con confidence >= 0.7"
  Proceso: "Clustering por dominio + tags + trigger similarity"
  6 outputs (cajas amber con iconos):
    [S] Skill → crea SKILL.md
    [C] Command → crea /comando
    [A] Agent → crea agente especializado
    [R] Rule → passive rule automatica
    [E] Enrich → extiende skill existente
    [P] Promote → project → global

SECCION LATERAL DERECHA — "Token Optimizer" (caja glassmorphism)
  Barra de salud: GREEN | YELLOW | ORANGE | RED
  Metricas: "bytes/4 estimacion", "60% overlap = redundante"

Conectores entre secciones: flechas con label de datos que fluyen.
Formato: 1920x1350px (mas alto para acomodar las 3 secciones).
```

---

## Leccion 7: Hermes a fondo — tools, gateway, cron y multi-modelo
**Tipo de visualizacion**: Diagrama de arquitectura radial (hub & spoke)

```
PROMPT — Plataforma: Figma

Crea un diagrama de arquitectura radial (hub and spoke) sobre fondo oscuro (#0a0a14).

CENTRO (hub grande, purple #7c3aed con glow):
  "HERMES AGENT"
  Subtitulo: "CLI + 40 tools + multi-modelo"

SPOKE 1 — ARRIBA (purple claro):
  "15+ Providers"
  Sub-nodos en abanico: Anthropic, OpenAI, OpenRouter, Ollama, Nous, Custom...

SPOKE 2 — ARRIBA DERECHA (blue #4a9eed):
  "Gateway — 9 plataformas"
  Sub-nodos: Telegram, Discord, Slack, WhatsApp, Signal, Email, SMS, DingTalk, Feishu

SPOKE 3 — DERECHA (amber #f59e0b):
  "Cron Scheduling"
  Sub-nodos: "Daily checks", "Weekly reports", "Deploy monitors"

SPOKE 4 — ABAJO DERECHA (green #22c55e):
  "Terminal Backends"
  Sub-nodos: Local, Docker, SSH, Daytona, Modal, Singularity

SPOKE 5 — ABAJO (teal #0d9488):
  "Skills Hub"
  Sub-nodos: "Marketplace", "Security scanning", "SKILL.md format"

SPOKE 6 — ABAJO IZQUIERDA (pink #ec4899):
  "Protocols"
  Sub-nodos: "MCP (Model Context Protocol)", "ACP (Agent Client Protocol)"

SPOKE 7 — IZQUIERDA (white/gray):
  "Tools nativos"
  Sub-nodos agrupados: terminal, web, vision, browser, file, tts, delegation, todo...

SPOKE 8 — ARRIBA IZQUIERDA (purple oscuro):
  "Profiles"
  Sub-nodos: "Multi-identidad", "Config aislada", "Skills separadas"

Lineas de conexion: solidas para features core, punteadas para opcionales.
Formato: 1920x1920px cuadrado (ideal para redes sociales).
```

---

## Leccion 8: La gran comparativa — cuando usar cada uno
**Tipo de visualizacion**: Tabla visual split (izquierda/derecha) con indicadores

```
PROMPT — Plataforma: Canva

Crea una infografia de comparativa split sobre fondo oscuro (#0a0a14).

TITULO: "Synapis vs Hermes: Cuando usar cada uno" (gradiente teal→amber→purple)

LAYOUT: 2 columnas con separador central amber punteado.

COLUMNA IZQUIERDA — SYNAPIS (fondo teal sutil):
  Header: "USA SYNAPIS cuando..." (teal bold)
  Items con icono ✓ teal:
    - Escribes/editas codigo en un proyecto
    - Quieres que tu AI aprenda tus patrones
    - Creas cursos, superskills, arquitectura
    - Haces code review, PRs, commits
    - Necesitas skills especializadas por proyecto
    - Quieres observacion pasiva y /evolve

COLUMNA DERECHA — HERMES (fondo purple sutil):
  Header: "USA HERMES cuando..." (purple bold)
  Items con icono ✓ purple:
    - Necesitas chat rapido en terminal
    - Quieres automatizar con cron jobs
    - Necesitas bot en Telegram/Discord
    - Usas modelos locales (Ollama) u OpenRouter
    - Investigas, buscas web, generas imagenes
    - Necesitas agente 24/7 en un VPS

SECCION INFERIOR — "POR QUE NO FUSIONAR" (fondo amber sutil):
  5 razones en cards horizontales con icono ✗ rojo:
    1. Dependes de 2 proyectos que no controlas
    2. Synapis funciona MEJOR como markdown (LLM interpreta > Python if/else)
    3. Hermes evoluciona rapido — plugins pueden cambiar en v1.0
    4. El overlap real es casi CERO en uso diario
    5. 4-5 semanas / 2400 lineas para reescribir algo que ya funciona

FOOTER: "La separacion ES la arquitectura correcta" (amber bold)

Formato: 1080x1920px vertical (ideal para historias de Instagram).
```

---

## Leccion 9: Scripts bridge — conectarlos sin fusionarlos
**Tipo de visualizacion**: Diagrama de secuencia bidireccional

```
PROMPT — Plataforma: Figma

Crea un diagrama de integracion bidireccional sobre fondo oscuro (#0a0a14).

3 COLUMNAS:
  - CLAUDE CODE + SYNAPIS (teal #0d9488)
  - SCRIPTS BRIDGE (amber #f59e0b, columna central destacada)
  - HERMES AGENT (purple #7c3aed)

FLUJO 1 — Izquierda a derecha (teal → amber → purple):
  "Desde Claude Code, consultar Hermes"
  Claude Code → bridge: ~/bin/hermes sessions list
  Bridge → Hermes: ejecuta y devuelve JSON
  Hermes → Claude Code: "Ultimas 5 sesiones resumidas"

FLUJO 2 — Derecha a izquierda (purple → amber → teal):
  "Desde Hermes, leer instincts de Synapis"
  Hermes → bridge: cat ~/.claude/skills/_instincts.json
  Bridge → Synapis data: lee JSON
  Synapis data → Hermes: "Tienes 6 instincts, 2 maduros"

FLUJO 3 — Bidireccional (amber central):
  "Compartir API keys sin duplicar"
  Caja izquierda: "Synapis hereda de Claude Code env"
  Caja derecha: "Hermes lee de su propio .env"
  Linea punteada central: "Misma ANTHROPIC_API_KEY, diferentes .env"

SECCION INFERIOR — "3 scripts listos para usar":
  Card 1 (amber): hermes-personal → "Chat personal con Anthropic"
  Card 2 (amber): synapis-project → "Lanza Claude Code + Synapis"
  Card 3 (amber): dual-status → "Estado de ambos lado a lado"

Formato: 1920x1080px horizontal.
```

---

## Leccion 10: Un dia con los dos agentes
**Tipo de visualizacion**: Timeline horizontal con iconos por herramienta

```
PROMPT — Plataforma: Canva

Crea una timeline horizontal de un dia completo sobre fondo oscuro (#0a0a14).

TITULO: "24 horas con Synapis + Hermes" (gradiente teal→purple)

TIMELINE de izquierda a derecha con hora y actividad:

08:00 (purple, icono cafe+terminal):
  "HERMES: Buenos dias"
  "hermes-personal → agenda, emails, research rapido"

09:00-12:00 (teal, icono codigo):
  "SYNAPIS + CLAUDE CODE: Desarrollo"
  "Escribir codigo → Synapis observa → Skills on demand"
  Barra ancha para indicar duracion larga

12:00 (teal, icono cerebro):
  "SYNAPIS: /instinct-status"
  "Ver patrones detectados en la manana"

14:00-17:00 (teal, icono codigo):
  "SYNAPIS + CLAUDE CODE: Mas desarrollo"
  "Code review, PRs, commits → Synapis sigue aprendiendo"

17:00 (amber, icono engranaje):
  "BRIDGE: Sincronizar"
  "hermes chat -q 'lee mis instincts de synapis'"

18:00 (purple, icono reloj):
  "HERMES CRON: Automatizacion"
  "Check de deployments, git log summary, health checks"

21:00 (purple, icono antena):
  "HERMES GATEWAY: Bot activo"
  "Telegram/Discord responde mensajes mientras duermes"

23:00 (teal, icono flecha circular):
  "SYNAPIS: /evolve (semanal)"
  "Patterns maduros → Skills nuevas → Tu Claude Code mejora"

Codigo de colores en leyenda inferior:
  Teal = Synapis/Claude Code | Purple = Hermes | Amber = Bridge

Formato: 1920x600px panoramico (ideal para header de web).
```

---

## Leccion 11: Extensiones avanzadas y futuro
**Tipo de visualizacion**: Diagrama de arquitectura con conexiones futuras (roadmap visual)

```
PROMPT — Plataforma: Figma

Crea un diagrama de arquitectura futura sobre fondo oscuro (#0a0a14).
Estilo: nodos existentes solidos + nodos futuros con borde punteado.

CAPA SUPERIOR — "HOY" (nodos solidos):
  Caja teal: "Synapis v3.2" con sub-items: skills, instincts, /evolve
  Caja purple: "Hermes v0.6" con sub-items: tools, gateway, cron
  Conexion amber solida: "Bridge scripts"

CAPA MEDIA — "EXTENSIONES POSIBLES" (nodos con borde punteado):
  Nodo 1 (teal punteado): "Skills de Hermes que delegan a Claude Code"
    Ejemplo: "hermes ejecuta → claude --print 'refactoriza X'"
  Nodo 2 (purple punteado): "Skills de Synapis que consultan Hermes"
    Ejemplo: "Desde Claude Code → hermes sessions list --json"
  Nodo 3 (amber punteado): "MCP Server compartido"
    Ejemplo: "Base de datos o API custom accesible desde ambos"
  Nodo 4 (green punteado): "Pipeline: Synapis detecta → Hermes ejecuta"
    Ejemplo: "Instinct maduro → cron job automatico"

CAPA INFERIOR — "FUTURO LEJANO" (nodos fantasma, opacidad 30%):
  Nodo: "Sincronizacion de memorias bidireccional"
  Nodo: "Hermes como plugin runtime para Synapis skills"
  Nodo: "Fusion como producto open source (si tuviera sentido)"

NOTA en esquina: "Cada capa es opcional. La arquitectura dual funciona perfectamente sin ninguna extension."

Formato: 1920x1350px vertical.
```

---

## Leccion 12: Proyecto final — tu setup personalizado
**Tipo de visualizacion**: Checklist visual gamificado con progreso

```
PROMPT — Plataforma: Canva

Crea un poster de proyecto final gamificado sobre fondo oscuro (#0a0a14).

TITULO: "Proyecto Final: Tu Setup Dual" (gradiente teal→amber→purple)
SUBTITULO: "5 entregables para graduarte como Maestro Dual"

5 CARDS VERTICALES con barra de progreso lateral:

CARD 1 (teal, icono verificacion):
  "Verificar instalacion"
  - hermes doctor → todo verde
  - Claude Code + Synapis cargando
  - Provider: Anthropic en ambos
  XP: 15 | Nivel: Basico

CARD 2 (amber, icono scripts):
  "3 Bridge Scripts"
  - hermes-research (Hermes investiga → archivo para Claude Code)
  - synapis-export (exporta instincts → formato Hermes)
  - dual-status (estado de ambos lado a lado)
  XP: 25 | Nivel: Intermedio

CARD 3 (purple, icono reloj):
  "1 Cron Job en Hermes"
  - Tarea diaria automatica
  - Output a log file
  - Ejemplo: resumen git de todos tus repos
  XP: 20 | Nivel: Avanzado

CARD 4 (teal, icono estrella):
  "1 Skill Custom en Synapis"
  - Resuelve un problema real de tu workflow
  - Formato SKILL.md con frontmatter
  - Registrada en _catalog.json
  XP: 20 | Nivel: Intermedio

CARD 5 (amber, icono documento):
  "Documentar tu setup"
  - Donde esta todo
  - Como arrancar cada herramienta
  - Como actualizar
  - Troubleshooting
  XP: 10 | Nivel: Basico

BARRA INFERIOR: "Total: 80 XP → Badge: Maestro Dual 👑"

Formato: 1080x1920px vertical (ideal para poster imprimible).
```

---

## Notas para el diseñador

### Paleta de colores consistente
| Elemento | Color | Hex |
|----------|-------|-----|
| Synapis | Teal | #0d9488 |
| Hermes | Purple | #7c3aed |
| Bridge/Fusion | Amber | #f59e0b |
| Fondo | Dark | #0a0a14 |
| Superficie | Surface | #111118 |
| Texto principal | Light | #e4e4eb |
| Texto secundario | Muted | #9999a8 |
| Exito | Green | #22c55e |
| Error/Warning | Red | #ef4444 |

### Tipografia
- **Titulos**: Outfit (800 weight)
- **Cuerpo**: Outfit (400 weight)
- **Codigo/tecnico**: Space Mono (400/700)

### Formatos recomendados
| Uso | Formato | Dimensiones |
|-----|---------|-------------|
| Web/curso | Horizontal | 1920x1080px |
| Stories/movil | Vertical | 1080x1920px |
| Redes sociales | Cuadrado | 1920x1920px |
| Panoramico/header | Wide | 1920x600px |
| Poster imprimible | Vertical | 1080x1920px |
