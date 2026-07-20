# Don Noel Projects Theme

This repository is the shared Jekyll remote theme for Don Noel project sites.

## Requirements

- Keep the theme usable by every approved project site; project-specific content stays in the consuming repository.
- Preserve the unique `assets/css/project-house.css` asset name. GitHub Pages reserves or generates `assets/css/style.css` for its default theme, so reusing that path can silently replace this theme.
- Make small, backward-compatible changes and validate them against at least one consuming site before tagging a release.
- Treat published version tags as immutable. Consumers should pin a release tag and upgrade deliberately.
- Keep the output accessible: semantic landmarks, visible keyboard focus, useful link names, readable contrast, responsive layouts, and reduced-motion support.
- Do not add JavaScript, analytics, external fonts, or third-party dependencies without explicit approval.

## Validation

- Build a consuming site with Jekyll.
- Check desktop and narrow layouts for horizontal overflow.
- Verify the generated page links to `project-house.css` and that the deployed stylesheet contains this theme's custom properties.
