# CLAUDE.md — Cosoteca (Obrero)

## Rules

### Placeholder text
Always use **lorem ipsum** for any placeholder, sample, or filler text. Never write "coming soon", "insert text here", or custom filler prose.

### Templates
Always use Zola templates. Never write inline HTML in content files beyond what Zola shortcodes require. All pages must extend `base.html` or a section-specific template.

### Partials
Every reusable UI module must live in `templates/partials/`. Create a new partial file whenever a pattern is used more than once or represents a distinct UI component (e.g. card, hero, nav, footer). Include partials with:

```jinja2
{% include "partials/component.html" %}
```

## Structure

```
templates/
  base.html              # root layout
  index.html             # home page (extends base)
  cosoteca/
    section.html         # cosoteca index (extends base)
    page.html            # cosoteca entry (extends base)
  partials/
    header.html          # site header + nav
    footer.html          # site footer
    hero.html            # hero banner module
    card.html            # content card module
    breadcrumb.html      # breadcrumb nav

content/
  _index.md              # home page
  cosoteca/
    _index.md            # cosoteca section index
    *.md                 # individual cosoteca entries
```
