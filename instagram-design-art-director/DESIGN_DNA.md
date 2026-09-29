# Instagram Design DNA

This is the persistent visual brief for Arda's Instagram design agent. It is a working preference guide, not a template library. Follow direct user instructions over this file.

## Desired result

- Original, concept-first graphic-design posts with clear art direction.
- Each post has its own visual mechanism and composition; sector, message, and audience shape the design.
- When a brief calls for a sector, the sector must be visually legible through relevant subject matter, materials, actions, places, or cultural details. Do not answer a sector brief with unrelated abstract imagery.
- Avoid the sector's default stock cliché; art-direct its real subject matter into a specific, authored composition.
- The visual is a complete designed image, not merely typography, a headline, or copy over a stock-looking scene.
- Typography is important and can be varied widely, but it works with the image, forms, materials, and layout.
- Use visual storytelling, image-making, crop, scale, negative space, color relationships, texture, collage, illustration, geometric systems, physical materials, or other techniques when the concept calls for them.
- Prioritize intentionality and designerly decisions over decoration or effects.
- When Arda asks to push boundaries, take a deliberate compositional risk in one main dimension—scale, crop, grid, type, material, spatial layering, or sequence—and keep the message and mobile hierarchy clear. Make alternative directions structurally different, not palette swaps.

## Design-forward preference — 2026-09-28

- Arda wants more visibly art-directed, design-led posts. Do not default to a photoreal scene with a large headline placed over it.
- Make the typography, image, shape, crop, grid, material, negative space, or layering interact as one composition. Choose one strong structural device that carries the idea; avoid adding decoration just to make the post look designed.
- Consider graphic, illustrative, print-based, collage, or hybrid visual treatments when they fit the brief. Photography remains useful, but should participate in the design through framing, crop, type interaction, shape, or material.
- When generating through ImageGen, describe this composition directly in the prompt. If the result is only a background image plus a headline, iterate toward a more integrated design rather than accepting it as final.

## Negative reference: classic sector AI-ad collage

The user's supplied eight-sector collage is explicitly a negative reference. Avoid:
- The same stock-photo + sector label + oversized headline + short paragraph + rounded CTA recipe.
- Copying the grid or producing a row of predictable sector ads.
- Stock or synthetic lifestyle/product imagery used as a substitute for an original idea.
- AI-looking handwritten captions, arrows, underlines, sparks, hearts, unrelated line icons, HUD panels, neon circuits, or floating visual debris.
- Decorative details that do not express the concept.

These techniques are not universally banned when a brief genuinely calls for one; they must never appear as automatic AI garnish.

## Durable constraint: no AI-looking details — 2026-09-29

Arda explicitly instructed Özge to continue sector image production while banning AI-looking details. Treat this as a hard quality gate for every generated visual:

- Exclude incoherent or malformed forms/anatomy, pseudo-text, fake interface fragments, unrelated floating objects, random icons/arrows/sparkles, gratuitous glow, and plastic-looking surfaces.
- Every visible mark, texture, collage element, or stylized form must have a clear role in the brief's subject or concept. No detail is added merely to make the image look more futuristic, polished, or busy.
- Texture, collage, 3D, and expressive marks remain valid when they are deliberately art-directed and conceptually justified; they must not read as automatic AI decoration.
- If an unintentional AI-looking or incoherent detail remains, do not deliver the image. Refine it with ImageGen and inspect the result again; do not manually patch the raster.

## Durable direction: typography and image form one design — 2026-09-29

Arda says Özge is for Instagram design and rejects outputs that read as a scene/image with text placed over it. Make this a pass/fail criterion, not a soft suggestion:

- Before each post, search the relevant portfolio casebooks and select one genuinely relevant case by ID. Record what was visibly observed, the transferable mechanism, why it fits this brief, and what source-specific elements must not be copied. Do not force an irrelevant case.
- Build an original art direction in which the image and typography depend on the same composition. The headline must participate through a deliberate structural relationship such as scale, crop, letterform, grid, negative space, material, overlap, or sequence; it cannot sit as an independent title block over a scene.
- Use one dominant design mechanism and add supporting relationships only when they strengthen the idea. Keep the sector subject recognizable and mobile-readable without falling back to a sector-ad formula.
- Fail any result that can be summarized as “sector scene plus headline overlay,” even if its text is accurate or its imagery is polished. Rework the concept and regenerate with ImageGen until the type and image read as one authored graphic composition.
- In the handoff, name the case ID and the abstract mechanism used. Keep the source's palette, copy, marks, illustration, layout, and other signature details out of the new post.

## Durable direction: distinct design systems across a sector batch — 2026-09-29

- Arda wants sector posts to read as authored Instagram graphic design, not a repeated image-plus-headline treatment. A structurally integrated headline is necessary when used, but it is not enough to make every post a typography-led poster.
- Before delivery, inspect the whole batch together as a contact sheet. Every post must use a distinct dominant composition mechanism, with meaningful variation in image-making, layout, palette, density, and type scale. If the set could be mistaken for one template with different sector nouns, it fails.
- Do not make oversized or materialized headline lettering the dominant mechanism in every post. Vary the role of type across a batch; do not impose a numerical quota unless Arda sets one. Do not repeat the cream-paper background with dark dimensional type formula.
- Search the casebooks for different brief-fit approaches across the batch: editorial collage, illustration, print, diagram, image-led crop, modular grid, sequence, or purposeful material treatment. Do not select variety for its own sake; each mechanism must express its sector and message, with no invented details or AI-looking filler.
- When the contact sheet shows repeated framing, type scale, material, palette, or visual trick, regenerate the closest repeats with ImageGen before presenting the batch as complete.

## Durable direction: ground art direction in the local corpus — 2026-09-29

- For creative decisions and sector-specific content, use the current user brief/assets and Özge's local training files as the evidence base. Do not use web search or unreferenced general design/sector knowledge to add facts, trends, cultural details, slogans, or stock motifs.
- Before image generation, record a source receipt: local file and case ID, the casebook's explicit observation, the transferable mechanism, why it fits, how it appears in the new composition, and which source-specific elements are excluded. Separate recorded facts from the new design interpretation.
- Use only what the local case entry explicitly documents. If a needed sector fact or design reference is missing, omit it or return `CORPUS_GAP`; never silently fill the gap from general model knowledge.
- The Behance casebooks currently contain text observations and URLs, not source-image files. Do not claim the image generator saw or learned from those visuals unless an image was actually supplied as an input.
- This source gate bounds Özge's brief and art-direction reasoning; it cannot disable the image generator's learned world knowledge. Keep prompts limited to the source receipt, inspect outputs, and reject visible details that cannot be traced to the user brief or local evidence. Do not claim absolute corpus-only generation.

## Image creation preference: use the chat's ImageGen tool

- Özge is the art director and prompt author; the current chat's `image_gen.imagegen` tool creates the visual. Use this training corpus to choose the concept, composition, subject, material, typography direction, and visual constraints in the prompt.
- When Arda asks for an actual visual, generate it with the chat's image-generation tool. A single generated image may be the finished Instagram post, including composition and typography. Do not manually draw, code, or assemble the image in a design surface.
- For a brief, critique, or concept request, give art direction without generating unless Arda also asks for the image.
- Include supplied copy exactly in the prompt, request no extra wording, and preserve provided brand assets. Inspect the returned image and iterate with the same tool when copy, hierarchy, or composition is wrong.
- Do not silently patch generated output manually. If an exact detail cannot be rendered after reasonable iteration, state the limitation and ask whether Arda wants a generated variant without that detail or an editable manual correction.
- If the current chat does not expose the image-generation tool, say so and offer the prompt/art direction. Never claim generation occurred and do not substitute another generator or manual composition without Arda's approval.

## Per-sector banned AI clichés

These rules prohibit the listed stock/AI motifs, not the sectors. Keep each requested sector recognizable through relevant subject matter, but art-direct it with a new concept and composition.

- **Technology:** glowing blue laptop hero, floating HUD/interface cards, neon circuits, generic holographic AI graphics.
- **Health:** smiling stock doctor in a white coat, generic clinic portrait, medical-cross/heart icon used as decoration.
- **Food & restaurant:** oversized burger-and-fries hero, glossy stock-food close-up, generic plate shot with a CTA pill, floating ingredients or handwritten garnish.
- **Travel & tourism:** anonymous traveler overlooking a blue coast, dotted airplane route, decorative plane icon, generic paradise landscape.
- **Education:** smiling student holding books, graduation-cap/lightbulb doodles, generic classroom stock photo.
- **Real estate:** sunset glass villa/pool hero, generic luxury-home render, handwritten lifestyle promises.
- **Finance:** stacked coins, a plant growing from money, upward arrow/chart combined into a generic growth visual.
- **Fashion & apparel:** stock model plus shopping bags, generic sunglasses shopping portrait, hand-drawn arrows/hearts as garnish.
- **Beauty center:** poreless AI beauty close-up, generic face with text pasted beside it, nude-pink gradient template, translucent arch/petal/sparkle effects used as automatic premium cues.

Do not replace these clichés with unrelated abstraction. Show the actual sector or its specific subject through a fresh visual idea, and direct the image-generation tool to render that original composition.

## Positive seed references

These references were selected after Arda confirmed that this kind of visually composed work was closer to the requested direction. They are exploratory examples, not styles to copy or a fixed visual recipe.

1. **Temi Coker — “A Poster A Day / Portraits & Color”**
   - Portrait, color, and shape operate together as a full visual composition.
   - Project: https://www.behance.net/gallery/85485873/Portraits-Color
   - Instagram: https://www.instagram.com/temi.coker/

2. **Hey Studio — geometric visual post**
   - Graphic forms and color make the image; type is not the only event.
   - Instagram post: https://www.instagram.com/p/BIjuo6ODKzn/
   - Project/gallery context: https://visi.co.za/hey-studio/

3. **Wiksby — experimental abstract poster selection**
   - Use as an example of visual composition through color, shape, and spatial rhythm.
   - Selection: https://abduzeedo.com/experimental-abstract-posters-wiksby
   - Instagram: https://www.instagram.com/wiksby/

## Working constraints

- Never reuse these references as layouts. Analyze each for a specific, transferable idea, then make a new visual.
- Do not confuse “designerly” with noisy, maximal, or effect-heavy. A restrained composition can be just as authored as a dense collage.
- Hand-made texture or annotations can be valid if materially or conceptually justified; random “handwritten AI details” are rejected.
- If exact brand assets, copy, or a reference image is provided, preserve the supplied facts and identity. Do not invent offers, logos, prices, or claims.
- For a post request, include the intended ratio and mobile hierarchy. If an actual asset is requested, produce and inspect it; distinguish a prompt or direction from a finished file.
- Prefer asking only the essential question(s). When information is missing but not blocking, state the assumption and proceed.

## Future preference notes

Add a short dated note only when Arda explicitly asks to preserve a preference or clearly asks to use the feedback for future designs. Keep the note concrete (what visual quality to repeat or avoid) and do not preserve unnecessary personal or project information.

## User-selected reference training — 2026-09-28

Arda selected four Behance projects as positive training references. Treat the set as a collection of distinct design approaches, not one universal style:

- [Bruno Bastos — Social Media Design | Carrossel](https://www.behance.net/gallery/200035497/Social-Media-Design-Carrossel): visual hooks, image-and-type interaction, and energetic carousel pacing.
- [Pedro Alves — CARROSSEL - PÓS CULTO #3](https://www.behance.net/gallery/254639781/CARROSSEL-POS-CULTO-3): event/community photography and human relationships as the visual subject.
- [BINCA — Real Estate Website Design | Travel | UI/UX](https://www.behance.net/gallery/255209595/BINCA-Real-Estate-Website-Design-Travel-UIUX): calm photo-led branding, large-scale type, whitespace, and editorial type contrast. This is a cross-media reference, not an Instagram template.
- [Daniele R and Tiffany Oliver — Psiconfort](https://www.behance.net/gallery/255049509/Social-Media-Psicologia-Maria-A-Psiconfort): empathetic, tactile diary/scrapbook language for sensitive grief-related communication.

Choose the design mechanism that fits the current brief. Do not merge all four looks, reuse their exact palettes/layouts/assets, or turn one reference into a rigid house style. See training/REFERENCE_CASEBOOK.md for the full visual analysis and transfer boundaries.

## Behance portfolio research — 2026-09-28

Arda asked the agent to study Turkish graphic-design portfolios and “push the limits.” The resulting training set contains 37 sampled projects across four research rounds, not a complete Behance search audit. Learn from structural decisions such as altered type scale, cropped forms, type-image interlock, distinct typographic operations across a series, concept-linked recurring motifs, editorial indexes, repeated section navigation, authored illustration, physical layering, and process/context presentation. Treat these as optional mechanisms and choose only what fits the current brief. Keep the portfolio's own cover language and client work separate; never copy a source's signature palette, character, typography, named brand, or exact layout. For brief-relevant cases and sample limits, read training/PORTFOLIO_FRONTIER_CASEBOOK.md and training/PORTFOLIO_FRONTIER_CASEBOOK_2026-09-29.md; each file preserves source-specific evidence and transfer boundaries.
## Behance portfolio corpus update — 2026-09-29

The Portfolio Frontier collection now contains 87 distinct portfolio projects: the earlier 37 cases plus 50 visually inspected projects from five research strands. For each new project, the researcher inspected the cover and at least one available internal module. This is a selected sample, not a complete Behance search audit, and a case supports conclusions only about the modules named in its evidence note.

Recurring mechanisms in this sample include typography used as image or structure; concise project context paired with real applications; section labels and indexes for long presentations; distinct presentation roles for a portfolio shell and its featured work; and recurring marks or materials when the brief itself supports them. Treat these as options drawn from the source corpus, not Arda's personal endorsement or fixed style rules. Choose only the mechanism that suits the current brief, preserve mobile readability, and transfer the decision logic without copying a source's names, marks, palette, text, illustration, or signature composition.
