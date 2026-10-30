# Neonverse — Responsive Product Landing Page

Neonverse is a fictional immersive-technology studio that creates interactive virtual worlds. This project was designed as an individual UI/UX landing-page submission and implemented as a responsive React website.

## Intended users

The primary audience is people aged 18–35 who are interested in virtual reality, gaming, interactive art, and emerging technology. Secondary users include creative studios and brands looking for immersive digital experiences.

## Design choices

- **Visual direction:** A deep plum background with cyan, violet, and magenta accents creates a futuristic atmosphere without reducing readability.
- **Typography:** Space Grotesk is used for expressive display headings, while Manrope keeps navigation and body content clear.
- **Hierarchy:** The oversized hero statement establishes the product immediately, followed by one primary action and three scannable product benefits.
- **Layout:** Grid and flex layouts provide the same content hierarchy across desktop, tablet, and mobile screens.
- **Interaction:** Hover feedback, subtle floating motion, smooth navigation, and reduced-motion support create a polished but accessible experience.

## Reusable components

1. `PrimaryButton` — the primary call-to-action used for “Explore worlds.”
2. `NavigationLink` — reusable header navigation item.
3. `FeatureCard` — the featured immersive-world visual.
4. `ProductFeatureCard` — reusable product benefit card rendered three times from shared data.

## Shared styles

Color and typography values are defined as shared CSS custom properties in `src/index.css`. Consistent spacing, borders, card treatments, and responsive breakpoints are reused throughout the page.

## Generate the native Figma design

The repository includes a development plugin that creates the assignment as a fully editable Figma design. It generates:

- A 1440 px desktop landing-page frame
- A 390 px mobile responsive frame
- Auto Layout for the header, navigation, hero content, feature section, cards, buttons, and footer
- Native `Button / Primary`, `Navigation / Link`, and `Card / Feature` components
- Component instances with editable text overrides
- Shared Neonverse paint and typography styles
- An original abstract VR illustration

To run it:

1. Open the **Figma desktop app** and create or open a Design file.
2. Open **Plugins → Development → Import plugin from manifest**.
3. Select `figma-plugin/manifest.json` from this repository.
4. Run **Plugins → Development → Generate Neonverse Assignment**.
5. Save the generated Figma file and enable link sharing for your submission.

The generated desktop and mobile frames are native Figma layers—not flattened images—and can be inspected for Auto Layout and component usage.

## Run locally

```bash
pnpm install
pnpm dev
```

Create a production build with:

```bash
pnpm build
```
