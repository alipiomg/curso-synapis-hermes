# Changelog — Sinapsis + Hermes: Domina tus dos agentes AI

## [1.1.0] — 2026-03-31

### Actualizado
- Renombrado "Synapis" → "Sinapsis" en todo el curso (alineado con branding oficial)
- Leccion 6 reescrita con la evolucion v3.2 → v4.1:
  - Pipeline cerrado de 6 pasos (observe→learn→propose→confirm→inject)
  - 3 niveles de confianza (draft/confirmed/permanent) reemplazan scoring 0.0-1.0
  - Context.md entre sesiones (session-learner + project-context)
  - Domain dedup: max 1 instinct por dominio, max 3 simultaneos
  - Sin ruido: de 80+ propuestas/dia a solo error→solucion real
- Instalacion rapida con prompts copy-paste para Claude Code (en vez de comandos bash)
- Landing con hero video background (lazy load + dark overlay)
- Sistema de superpoderes con 9 misiones por niveles + escalera de valor
- Navbar premium con hover effects
- Version del curso: 1.0.0 → 1.1.0

### Fuentes
- sinapsis-v4-comparison.html (documentacion tecnica v4.1 de SalgadoIA)
- synapsis-evolution-non-technical.html (explicacion no-tecnica del Learning Engine v3)

## [1.0.0] — 2026-03-30

### Creado
- course.json con 12 nodos, 3 rutas pedagogicas, 7 zonas
- 12 microlecciones en concepts/ con 6 secciones cada una
- gamification.json: 5 niveles, 8 badges, XP config
- observables.json: 7 eventos trackeables para Sinapsis
- prompts.md: 12 prompts de infografia con tipos de visualizacion especificos
- COURSE-PEDAGOGY.md: patrones pedagogicos documentados
- Sistema de niveles alternantes (basico→avanzado→intermedio)
- Glosario progresivo (cada termino se explica una sola vez)
- Tesis central: "No fusionar, conectar via bridge scripts"

### Decisiones de diseno
- 12 nodos (dentro del rango 8-15 recomendado por Course Architect)
- Alternancia de niveles para mantener engagement
- La leccion 8 (comparativa) es el nodo central del curso
- Proyecto final con 5 entregables que cubren todos los niveles
- Colores: teal (Sinapsis) + purple (Hermes) + amber (bridge)
