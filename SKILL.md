---
name: ai-architecture-visuals
description: Generate or transform architectural project imagery into 12 specific diagram and rendering types, including site analysis, massing, axonometric, collage, competition render, illustration, and physical-model looks. Use when a user wants AI-assisted architecture presentation images; do not use for dimensionally authoritative construction drawings or code-compliance documentation.
---

# AI Architecture Visuals

Create presentation-ready architectural visuals while preserving the designer's geometry, spatial logic, and authorship.

## Workflow

1. Identify the requested visual type(s) from the 12 modes in [references/prompt-library.md](references/prompt-library.md). Read only the selected mode sections; read all sections only when the user requests the complete 12-image set.
2. Inventory the supplied evidence: site/aerial image, plan, section, axonometric, massing model, SketchUp screenshot, render, material palette, labels, and desired aspect ratio.
3. Separate invariants from styling:
   - Invariants: footprint, massing, openings, circulation, terrain, camera, scale relationships, and required program.
   - Styling: palette, texture, atmosphere, vegetation, entourage, diagram language, and graphic layout.
4. If a transformation needs source geometry but none is supplied, ask for the minimum missing source image. If the request is conceptual and geometry is intentionally open, proceed from the written brief.
5. Build a generation prompt by filling the selected template's variables. State invariants before visual style. Include an explicit negative block.
6. Use image editing/reference-image generation when preserving an input; use text-to-image only for genuinely new conceptual visuals.
7. For diagrams with precise labels, generate the clean diagram base first, then add verified text with a layout-capable tool. Never rely on raster image generation for final small text.
8. Inspect the result against the mode's acceptance checks. Iterate only on failed criteria and keep successful geometry fixed.

## Guardrails

- Do not invent dimensions, historical facts, site problems, program, or structural systems. Ask for or visibly mark unknown information.
- Do not silently alter user-authored plans, elevations, sections, footprints, or massing. AI may clarify or restyle them, not redesign them, unless explicitly requested.
- Do not present generated imagery as measured, permitted, buildable, or code-compliant documentation.
- Keep labels legible and factually grounded. Use placeholders such as `[LABEL]` when final copy is unavailable.
- Preserve the user's requested language, orientation, aspect ratio, and deliverable count.

## Complete Set

When asked for all 12 types, produce and name them in this order:

1. `01-mapping-base`
2. `02-history-culture-analysis`
3. `03-existing-conditions-analysis`
4. `04-concept-collage`
5. `05-massing-process`
6. `06-linework-colorization`
7. `07-exploded-axonometric`
8. `08-axonometric-scenes`
9. `09-form-extraction`
10. `10-competition-render`
11. `11-editorial-illustration-render`
12. `12-physical-model-render`

Maintain a shared palette, typography, line weight, margins, and caption system across the set unless the user asks for independent styles.
