# Nuralfian Rashid - Personal Portfolio & Knowledge Base

A zero-JS, manual multi-page HTML and CSS codebase serving as a personal portfolio and technical showcase.

## Architecture

This site is built strictly with native HTML5 and CSS. 
- **Zero JavaScript**
- **No Static Site Generators (SSG)**
- **No Build Tools**

All styling is unified under `/css/style.css`, which utilizes modern CSS custom properties (variables) for a consistent design system.

## Directory Structure

```text
.
├── css/
│   └── style.css          # Unified global stylesheet (design tokens, components)
├── case-studies/          # Directory for in-depth technical case studies
│   └── template.html      # Reusable boilerplate for new case studies
├── index.html             # Homepage / About / Portfolio overview
└── README.md              # Documentation
```

## Adding a New Case Study

1. Navigate to the `case-studies/` directory.
2. Duplicate `template.html` and rename it to your project name (e.g., `legacy-migration.html`).
3. Open the new file and update the content, adhering to the standard framework:
   - Overview / Context
   - System Architecture
   - Technical Challenges
   - Execution & Implementation
   - Results & Learnings
4. Ensure the CSS `<link>` tag correctly points to `../css/style.css`.
5. Open `index.html` in the root directory and add a new `<article class="card">` linking to your newly created case study HTML file.

## Maintenance

To update global styles (colors, typography, spacing), modify the `:root` variables at the top of `/css/style.css`. Because all pages link to this single CSS file, changes will propagate universally.
