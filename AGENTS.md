# AniLearn AI Development Rules

## Project purpose
AniLearn is a Traditional Chinese beginner-friendly interactive algorithm learning website. The initial lesson is Binary Search. Future lessons should be easy to add consistently.

## Stack and deployment
- Vanilla HTML, CSS and JavaScript only; no build step, backend or API keys.
- All asset paths must be relative so GitHub Pages works under a repository subpath.
- Deploy from the repository root on the main branch.

## Visual design
- Soft lavender, cream and white; clean rounded cards and generous spacing.
- Responsive on desktop and mobile; readable text and accessible buttons.
- Interface and explanations in Traditional Chinese; algorithm names may include English.

## Page structure
Each lesson must include: title (Chinese and English), concept, prerequisites, numbered steps, interactive demo or illustrated example, complexity, and common mistakes.

## Files
- `index.html`: homepage and lesson navigation.
- `style.css`: shared design tokens, layouts and components.
- `app.js`: lesson registry and interactive behaviors.
- `AGENTS.md`: these project rules.
- New lesson identifiers: lowercase kebab-case (e.g. `linear-search`).

## Adding a lesson
1. Add a lesson object to the `lessons` array in `app.js` with id, title, english, summary, concept, prerequisites, steps, complexity, mistakes and demo type.
2. Add or extend a demo renderer using safe DOM APIs; avoid `innerHTML` with user input.
3. Keep existing lessons and navigation working.
4. Check mobile layout, keyboard controls and clear error messages.
5. Never introduce paid dependencies or secrets without explicit approval.

## Quality checklist
- Homepage loads with no console errors.
- Every lesson can be opened and navigated back from.
- Demos validate inputs and show understandable feedback.
- Content is accurate and friendly to beginners.
- No absolute-root asset paths.
