# Preliminary fountain refinement

Roosters: warm sandstone with a rooster relief. Doms: pale stone, fluting and Art Deco diamond inlays. Bens: weathered teal stone, bronze nozzle and water-drop medallion. Freddo: green stone with paired frog-like medallions and leaf inlays. Ham Sandwich: pink sandstone, layered sandwich relief and diamond masonry details.

Artwork fills the original solid rectangles; decorative reliefs and basin-water highlights stay within those rectangles. No new scenery, animated water or protruding obstacles were added. Existing active jets remain drawn by the unchanged game renderer above the assets.

The first three SVGs share a 122 x 91 viewBox and map to the original level-specific destination bounds. Freddo uses 380 x 100, Ham Sandwich uses 640 x 105. All ART_ASSETS destination bounds are unchanged. The Ham Sandwich internal asset key remains ride-the-jets for compatibility.

The game embeds the SVGs as data URLs to remain a standalone offline HTML file. Update both the editable SVG and its embedded source when replacing art. Never derive collision geometry from image dimensions. Hitboxes debug remains available.

Archibald, Boz, hotel, controls and all gameplay code are unchanged. The sole text change uses MISSED HIM! for failed attempts with Hellmen Assist purchased; ordinary misses and OUT OF PINTS retain their existing messages and priority.

Validation: 2,549 existing gameplay checks plus 20 fountain checks passed. Full source comparison allows only the five fountain asset sources and the miss-message expression to differ from work/fountains-before-refinement.html. Preview was rendered from SVG geometry; live Chrome gameplay rendering was not inspected.
