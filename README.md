# Don Noel Projects Theme

The shared Jekyll remote theme for Don Noel project websites hosted on GitHub Pages.

The theme provides the common project masthead, footer, typography, color system, responsive layout, accessible focus treatment, cards, status surfaces, and reusable content sections. Each consuming repository owns its project-specific title, status, links, and page content.

## Use from a project site

Add the versioned remote theme to the consuming repository's `_config.yml`:

```yaml
remote_theme: donnoel/projects-theme@v1.0.1

plugins:
  - jekyll-remote-theme
```

The shared layout expects the normal project metadata:

```yaml
title: Project Name
description: Short project description.
tagline: Short footer tagline.
project_label: Don Noel / Projects
github_url: https://github.com/donnoel/ProjectName
url: https://donnoel.github.io
baseurl: /ProjectName
lang: en-US
```

Set `hide_github_link: true` when a project site should omit the repository link
from the shared header. The link remains visible by default for existing sites.

Project content should use `layout: default`. Keep project-specific content in the consuming repository.

## Release process

1. Validate theme changes locally against a consuming site.
2. Commit and push the theme change.
3. Tag a version such as `v1.1.0`.
4. Upgrade consuming repositories one at a time and visually approve each live site.

The stylesheet intentionally uses `assets/css/project-house.css`. Do not rename it to `style.css`; that path collides with GitHub Pages' generated default-theme stylesheet.
