# Kognati.github.io

Personal portfolio site. Static HTML/CSS/JS, no build step, no dependencies.

## Preview it locally

```
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

## Deploy

This repo is named `<username>.github.io`, so GitHub Pages serves it
directly from the root of the `main` branch once Pages is enabled:

`Settings → Pages → Source: Deploy from branch → main / (root)`

Push to `main` and the site goes live at `https://<username>.github.io`.

## Fill in your info

Everything that needs replacing is written as an uppercase
`{{PLACEHOLDER}}` token in `index.html` — search for `{{` to find every
spot, including:

- name, role, location, bio, and the hero meta row
- stack manifest (languages / frameworks / infrastructure / tooling)
- the four project "units" (name, description, tags, repo/live links)
- experience timeline rows
- contact links (email, GitHub, LinkedIn, resume)

## Design

Dark tactical-telemetry/industrial-brutalist style: monospace
(JetBrains Mono) for data and labels, a heavy grotesque (Archivo Black)
for the oversized section headers, hard 90° corners, grid-line
dividers. Three accent colors each have one job — amber for section
indices and highlights, green for "active/online" status, cyan for
links and hover states — so it reads sharp rather than flat black-on-
white. Colors and fonts are CSS custom properties at the top of
`style.css` if you want to retune them.
