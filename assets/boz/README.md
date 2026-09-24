# Boz refinement pass 1

Six vector poses: ready, aiming, flying, falling, impact (`lost`) and landing (`won`). All share the same head, torso, clothing and palette. Limb poses change only in the renderer; no bounce or other movement was added to the simulation.

Every SVG uses a 48 × 66 viewBox. The body origin is SVG coordinate (24,33), drawn at the original world bounds [-24,-33,48,66]. Collision dimensions, core hitbox and launch origin remain unchanged. Hitboxes debug remains available.

The game embeds these SVGs as data URLs so the HTML still works offline as one file. When editing an SVG, update its matching ART_ASSETS data URL too. Keep the destination bounds fixed; never derive physics from artwork.

Matching helmet variants use a fitted padded shell and chin strap. They are prepared assets only: this baseline has Hellmen Assist but no helmet state. No new helmet activation or assist behaviour was introduced.

The original canvas drawing remains the loading/error fallback. The pre-pass game is preserved in work/boz-before-refinement.html.

Validation: 2,549 existing gameplay checks passed, including successful routes through all six levels, input, collisions, jet contacts, assist, refills and ending/reset. Forty visual checks confirm fixed bounds, offline assets, pose selection and no simulation mutations. Source comparison limits changes to Boz registry entries and visual pose selection. Pose preview rendered from SVG geometry at enlarged and small sizes; live Chrome gameplay rendering was not inspected.
