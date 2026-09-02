# Prompt Library

These templates adapt the 12 architectural-image patterns from the user's reference into reusable, model-agnostic instructions. Replace bracketed variables with project facts. Do not send bracket placeholders to an image model unchanged.

## Shared Prompt Order

Compose each prompt in this order:

1. Task and source-image role
2. Geometry/content invariants
3. Composition and camera
4. Graphic or material treatment
5. Palette and lighting
6. Labels to reserve or overlay
7. Negative constraints

Shared negative block:

> Do not change the supplied footprint, massing, camera, circulation, terrain, or scale relationships. Do not invent program or site facts. No illegible text, fake dimensions, warped grids, duplicated elements, decorative clutter, watermark, logo, or unrelated objects.

## 1. Mapping Base

Use for converting an aerial or satellite base into a restrained planning map.

Required input: aerial/satellite image or georeferenced exported base.

Template:

> Re-render the supplied base map as a minimalist planar urban mapping diagram. Preserve every road alignment, shoreline, parcel boundary, building footprint, and spatial relationship. Use a monochrome light-gray-to-white base; buildings are the darkest tone, followed by vegetation and water, while roads remain white. Low contrast, clean vector-like linework, no texture or decoration, pure pale gray-white background, complete and legible urban fabric.

Acceptance: source orientation and topology match; roads, water, buildings, and open space remain distinguishable; no invented features.

## 2. History and Culture Analysis

Use for a chronological site narrative.

Required input: verified timeline, dated images, and event captions.

Template:

> Create a horizontal historical site-analysis collage for [SITE]. Use the verified dates [DATES] as a continuous timeline. At each node place its corresponding architecture or streetscape fragment and a short reserved caption area. Blend archival monochrome photographs with restrained contemporary imagery and representative people or activities from each verified period. Black, white, and gray base with low-saturation [ACCENT_COLOR] lines, frames, and dots; irregular collage crops; coherent left-to-right chronology; clean white background.

Acceptance: chronology is correct; each image belongs to its date; generated people do not assert unsupported historical facts; all final labels are overlaid separately.

## 3. Existing Conditions Analysis

Use for annotated streetscape or site-problem analysis.

Required input: site photograph and a verified list of conditions, constraints, opportunities, circulation, views, and landscape notes.

Template:

> Turn the supplied [STREET/SITE] photograph into a professional annotated existing-conditions analysis. Keep the photograph central and unchanged. Connect verified regions to surrounding annotation zones with crisp color-coded arrows. Reserve a compact legend at lower left. Use [COLOR_KEY] consistently for existing conditions, circulation, landscape, views, constraints, and opportunities. Apply only a subtle low-contrast wash to the photo; dark legible text; documentary architectural-competition layout; no decorative background.

Acceptance: every arrow lands on the correct feature; legend colors are consistent; no issue or opportunity is invented.

## 4. Concept Collage

Use for adaptive reuse, renewal, museum, park, or community narratives.

Required input: theme, verified before/after elements, stakeholders, program, and preferred organizing logic.

Template:

> Create a texture-rich architectural concept collage about [THEME]. Combine verified historical fragments, contemporary spatial scenes, distinct user groups, and program elements [PROGRAM]. Organize the narrative as [CIRCULAR CLUSTERS / LINEAR TIMELINE / OTHER LOGIC] so every image connects through one clear sequence. Use low-saturation documentary color with vintage paper and restrained [ACCENT_COLOR] rules, nodes, and reserved caption areas. Pure white background, clear hierarchy, no unrelated texture.

Acceptance: one readable story; each element has a reason to exist; past, present, intervention, and outcome are distinguishable.

## 5. Massing Process

Use for staged design evolution.

Required input: final massing or several verified design stages; camera view.

Template:

> Create a paired, horizontal staged massing-process diagram for [PROJECT] in a fixed axonometric view. Show [STAGE_COUNT] verified stages from basic gray volumes to [FINAL_FEATURES]. Align every stage to the same footprint and camera, connect stages with fine pale-gray guides, and preserve a continuous design narrative. Early stages use neutral geometry; later stages add only the documented openings, structure, terraces, roof landscape, streets, and planting. Low-saturation fresh palette, white background, crisp lines, flat color, reserved stage-title areas.

Acceptance: stages are true transformations rather than unrelated designs; camera and scale are constant; final massing matches the source.

## 6. Linework Colorization

Use for coloring plans or landscape line drawings.

Required input: clean line drawing.

Template:

> Colorize the supplied top-view [PLAN TYPE] without moving, deleting, or redrawing any linework, symbol, label position, or boundary. Apply a hand-rendered light-watercolor wash: layered light and dark greens for planting, warm pale gray-beige paving, muted blue-gray water, restrained material tones, and black sketch contours. Keep the white background and all design annotations readable. Natural, low-saturation, professional landscape-architecture presentation.

Acceptance: pixel-level layout is preserved; all paths, rooms, planting, and water remain in their original positions; wash does not obscure linework.

## 7. Exploded Axonometric

Use for component, enclosure, structure, or assembly diagrams.

Required input: axonometric or 3D view plus an accurate component hierarchy.

Template:

> Convert the supplied building axonometric into a precise exploded assembly diagram on a black dotted/isometric grid. Keep the same camera and footprint. Separate the documented components from bottom to top: [COMPONENTS]. Use light gray and white building elements for strong contrast, consistent vertical offsets, fine leader lines, and reserved label zones. Technical architectural drawing, exact alignment, clean hierarchy, no missing or duplicated parts.

Acceptance: layers can visually reassemble; separation order is correct; leaders point to one component each.

## 8. Axonometric Small Scenes

Use for program vignettes, learning scenes, community activities, or user journeys.

Required input: list of scenes and the concrete objects/activities in each.

Template:

> Create a vertical series of [COUNT] equal-size 2.5D isometric scene illustrations: [SCENES]. Use a consistent isometric camera and grid, evenly distributed objects, small simplified people performing the specified activities, and reserved functional captions. Restrained pale teal-green palette with white and light gray, flat minimal technology-editorial illustration, clean white background, consistent scale and line weight.

Acceptance: each scene is distinct and correctly programmed; camera, character language, palette, and scale are consistent.

## 9. Architectural Form Extraction

Use for comparing aerial photographs with abstract footprint diagrams.

Required input: aerial images and verified footprint/figure-ground masks.

Template:

> Create a two-tier architectural form-extraction board in a regular [COLUMNS]-column grid. For each site, place the grayscale aerial image above and its simplified solid-black footprint or figure-ground symbol below, with a reserved site-name area. Preserve each source footprint exactly. White background, pure black geometry, restrained grayscale aerials, generous spacing, rigorous analytical hierarchy, no ornamental graphics.

Acceptance: every symbol maps to its paired aerial; figure-ground shapes are faithful; grid and spacing are uniform.

## 10. Competition Render

Use for a restrained photoreal architectural visualization from a model or draft render.

Required input: model/render with fixed camera and intended materials.

Template:

> Produce a high-end architectural competition render from the supplied model without changing geometry, facade rhythm, openings, camera, or composition. [MATERIAL_SYSTEM]. Emphasize [DESIGN_QUALITIES]. Use soft diffuse daylight, subtle reflections, transparent interior depth, realistic but restrained vegetation and people, cool contemporary palette, quiet atmospheric background, precise structure, no dramatic fantasy effects.

For glass-and-grid modernism, `MATERIAL_SYSTEM` may be: highly transparent curtain wall, fine orthogonal mullion grid, slender columns and beams, and clear interior structure.

Acceptance: geometry overlays the source; material behavior is plausible; entourage supports scale without blocking the architecture.

## 11. Editorial Illustration Render

Use for converting a 3D screenshot or render into a soft collage-like architectural illustration.

Required input: source view whose layout and camera must remain fixed.

Template:

> Transform the supplied [SCENE] into a lightweight editorial collage illustration while preserving the exact layout, camera, paths, buildings, and program. Convert all elements to flat color blocks with simple linework. Use [PALETTE] for architecture, landscape, ground, and sky; layered low-saturation greens for trees; simplified people consistent with the illustration style; a few restrained contextual elements such as birds only if appropriate. Soft, clean, paper-like finish with no complex texture.

Acceptance: composition matches the source; every major object remains identifiable; palette is layered but controlled.

## 12. Physical Model Render

Use for turning a digital white model into a convincing photographed handmade model.

Required input: white/clay model render.

Template:

> Render the supplied white digital model as a photographed handmade architectural model while preserving every volume, void, terrain contour, and spatial relationship. Replace digital white material with [MODEL_MATERIAL], showing fine grain, cut edges, slight fiber or tool marks, natural seams at assembled parts, and subtle surface wear. Convert the terrain base to layered [BASE_MATERIAL]. Use warm directional studio light, soft realistic shadows, shallow material variation, and a dark neutral backdrop. No change to design geometry.

Suggested materials: pale basswood, chipboard, kraft card, white museum board, cork, or layered gray board.

Acceptance: handmade cues are subtle and physically plausible; edges and joints remain crisp; model geometry and terrain are unchanged.

## Batch Consistency Checklist

For a 12-image set, record and reuse:

- Project name and one-sentence design concept
- Master palette with hex values
- Typeface and label hierarchy
- Line-weight hierarchy
- Page size/aspect ratio and margins
- Fixed source orientation and camera per view
- Approved program names and terminology
- Shared negative constraints

Before delivery, verify naming, count, source fidelity, text legibility, factual grounding, and cross-image visual consistency.
