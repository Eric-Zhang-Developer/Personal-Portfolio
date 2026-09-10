# Working in this repo

Read [README.md](README.md) for setup, current features, editing paths, and known tooling gaps.

## Project content

- Project entries live in `src/app/projects/page.tsx` and follow `src/types/project.ts`. Add images under `public/project-icons/`.
- When adding or removing projects, update the hardcoded count in `src/components/core/hero-section.tsx` too.
- Demo and GitHub links are optional. Show only the actions available for a project; do not add placeholder links.
- Keep descriptions factual. Do not invent features, results, metrics, or personal contributions. Ask when those details are needed but missing.
- Use plain language, sentence case for descriptions, and correct technology names. Do not use em dashes in site copy or documentation.

## Design and navigation

- Follow the existing terminal styling and shared tokens in `tailwind.config.ts` and `src/app/globals.css` unless the task calls for a design change.
- Preserve mobile layouts and reduced-motion behavior when editing the hero, matrix background, or CSS animations.
- When changing routes, check navigation links, homepage command buttons and prompts, and other links to the old route.
- Booking lives at `/hire-me`; the email form lives at `/hire-me/email`.

## Making changes

- Keep edits focused on the task and preserve unrelated work in the working tree.
- Investigate dependency workarounds before changing them. The README records the known reason for `legacy-peer-deps`; do not assume it is still needed or safe to remove.
- Update the README when a change affects documented features, structure, or commands.
- Keep temporary implementation plans in the ignored `agent-stuff/` directory. Track planned work in GitHub issues.

## Verification

- For documentation-only changes, check facts, paths, links, and the diff. No application build is needed.
- For application changes, run `npm run build` and check the affected pages. Include mobile layouts for visual changes, navigation destinations for route changes, and reduced-motion behavior for animation changes.
- Do not submit the live contact form or book a real appointment just to test the UI.
- The lint script is currently outdated, as noted in the README. Report checks that fail or cannot run, including existing tooling problems; do not describe them as passing.
- Review the final diff for unrelated changes and summarize what changed and how it was checked.
