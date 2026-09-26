# Project guidance for Claude

## Design / frontend work — always use the image-to-code skill

For **any** visual or frontend task in this repo — building or redesigning a
website, landing page, hero section, marketing page, portfolio, product page,
UI, or component — invoke the `image-to-code-skill` and follow its workflow by
default. Do not start with freeform coding on visual tasks.

Apply it automatically; the user should not have to ask for it by name.

Workflow the skill enforces:
1. If image generation is available, generate the design reference image(s)
   first, then deeply analyze them (typography, spacing, color, components).
2. If image generation is not available in the current environment, apply the
   skill's art-direction, analysis, and anti-AI-slop rules as design guidance
   and build faithfully from a clearly reasoned design system instead.
3. Implement frontend that matches the reference/design system closely — clean
   hero, generous spacing, no cards-inside-cards, no AI-slop gradients.

Skip the skill only for purely technical, non-visual work (bug fixes, refactors,
build/config changes) or when the user explicitly provides a finished design
system to follow verbatim.
