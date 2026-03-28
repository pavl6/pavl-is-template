# Hugo Template

A minimal Hugo template with basic CSS, navigation, and template content structure.

## Quick Start

```
hugo server
```

## Structure

```
content/
  _index.md          # Homepage
  about.md           # About page
  blog/
    _index.md        # Blog listing (with RSS)
    example-post.md  # Example blog post
  resources/
    _index.md        # Resources listing (simple style)
layouts/
  _default/
    baseof.html      # Base template (nav, footer, CSS/RSS head)
    list.html        # List pages (dated or simple style via listStyle param)
    single.html      # Single content pages
  index.html         # Homepage template
  404.html           # 404 page
  partials/
    back.html        # "< Back" link to parent page
    metadata.html    # Page created/edited dates
    page-children.html  # Simple child page listing
assets/
  css/main.css       # Stylesheet
archetypes/
  default.md         # Default archetype for new content
```

## Customisation

- **Site title**: Change `title` in `hugo.yaml`
- **Navigation**: Edit the `menus.main` entries in `hugo.yaml`
- **Styling**: Edit `assets/css/main.css` — colours are defined as CSS custom properties in `:root`
- **New section**: Create `content/section-name/_index.md` and add a menu entry in `hugo.yaml`
- **List style**: Set `listStyle: simple` in a list page's front matter for a plain link list (no dates), or omit it for a dated listing
- **New post**: Run `hugo new blog/my-post.md` or create the file manually
