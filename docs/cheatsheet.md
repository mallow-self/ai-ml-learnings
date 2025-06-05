# Cheatsheet

---

## 🔧 Basic Configuration (`mkdocs.yml`)

```yaml
site_name: My Project Docs
site_url: https://example.com
site_description: Documentation for my AI/ML learning
site_author: Rishi

nav:
  - Home: index.md
  - About: about.md
  - ML:
      - Basics: ml/basics.md
      - Models: ml/models.md
  - AI:
      - Concepts: ai/concepts.md
      - Tools: ai/tools.md

theme:
  name: material  # Recommended theme
  palette:
    primary: blue
    accent: indigo
  font:
    text: Roboto
    code: Roboto Mono

docs_dir: docs
site_dir: site
```

---

## 🧩 Common Extensions

```yaml
markdown_extensions:
  - toc:
      permalink: true
  - admonition
  - codehilite:
      guess_lang: false
  - pymdownx.superfences
  - pymdownx.details
  - pymdownx.highlight
  - pymdownx.inlinehilite
  - pymdownx.emoji:
      emoji_generator: !!python/name:pymdownx.emoji.to_svg
```

!!! note
    this is a note - admonition

```markdown
Learn this
    ```python
    int a = 10
    ```
```

==highlight== or `==highlight==`

:smile: :rocket: :+1:

### Title {.my-class}

---

## 🚀 Plugins

```yaml
plugins:
  - search
  - mkdocstrings  # for API docs (e.g., Python)
  - git-revision-date
```

> Install with:
> `pip install mkdocs-material mkdocstrings mkdocs-git-revision-date-plugin`

---

## 📁 Directory Structure

```bash
project/
├── docs/
│   ├── index.md
│   ├── about.md
│   └── ml/
│       └── basics.md
├── mkdocs.yml
```

---

## 🖼️ Extra Options (for Material theme)

```yaml
extra:
  social:
    - icon: fontawesome/brands/github
      link: https://github.com/yourusername
```

---

## 📦 Deployment (GitHub Pages)

```bash
pip install mkdocs ghp-import
mkdocs build
ghp-import site
git push origin gh-pages
```

Or simpler with Material:

```bash
mkdocs gh-deploy
```

---

## 🌐 Serve Locally

```bash
mkdocs serve
```

---
