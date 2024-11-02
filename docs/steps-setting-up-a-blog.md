# Install Material Mkdocs

Checkout the Material Mkdocs Basic Blogs tutorial [^1].

Material Mkdddocs  documentation [^2]

---

## Environment 

- Create new `GitHub` Repo
- `git clone` - new repo

Set up Python virtual environment

    `python -m venv venv`
    `source venv/bin/activate`

Open the cloned directoy in `vscode` then:
- `mkdocs new .`
- `pip install mkdocs-material`

---

# Setting up a blog

```
[ ] plugins:
        - blog
```

```
[ ] nav:
    - index.md
    - Blog:
        - blog/index.md
        - blog dir: .
```
---

## posts

```
[ ] post:
    ├─ docs/
    │  └─ blog/
    │     ├─ posts/
    │     │  └─ hello-world.md
    │     └─ index.md
    └─ mkdocs.yml
```

```
---
date: 2024-01-31
    categories:
        - Hello
        - World
---
```

`Hello world!`

---

## nav

```
---
date: 2024-01-31
links:
  - plugins/search.md
  - insiders/how-to-sponsor.md
  - Nested section:
    - External link: https://example.com
    - setup/setting-up-site-search.md
---

# Hello world!
```

---

## linking

linking to a post

```
[Hello World!](blog/posts/hello-world.md)
```

linking from a post

```
[Blog](../index.md)
```

---

## pinning a post

```
[Blog](../index.md)
```

---

## meta.yml

define all front matter
properties that are valid in posts

```
authors:
  - squidfunk
categories:
  - Hello
  - World
```

```
plugins:
  - meta
  - blog 
```

---

## adding pages

```
nav:
  - Blog:
    - blog/index.md
    - blog/authors.md
      ...
```

---
---

# material mkdocs categories

```
pip install mkdocs-categories-plugin
---
date: 2024-01-31
categories:
  - Hello
  - World
---
# Hello world!
```

---

```
plugins:
    - categories
    - search
    - blog:
        archive_date_format: MMMM yyyy
        categories_allowed:
            - Holidays
            - News
```

---

## front matter

```
---
categories:
  - Novels
  - Fiction
  - 19th Century Gothic Fiction
---
```

```
plugins:
  - categories:
      generate_index: true
      section_title: 'Categories'
      category_separator: '|'
```

---

## Footnotes

[^1]: [Material for MkDocs Basic Blog Tutorial](https://squidfunk.github.io/mkdocs-material/tutorials/blogs/basic/?h=blog)

[^2]: [Material for MkDocs Documentation](https://squidfunk.github.io/mkdocs-material/)
