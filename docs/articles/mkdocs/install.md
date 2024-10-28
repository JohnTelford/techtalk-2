---
date:
    created: 2024-10-21
categories:
    - Install
---

# Install Material Mkdocs Blog

October 20, 2024

> Website is being created using `VScode` [^1], `Marked 2 Steaming Preview` [^2], `Material for MkDocs` [^3], `Github` [^4]

- Checkout the Material Mkdocs Basic Blogs tutorial [^5].
- Material Mkdddocs  documentation [^6]


## Environment 

- Create new `GitHub` Repo
- `git clone` - new repo

Set up Python virtual environment

    `python -m venv venv`
    `source venv/bin/activate`

## Install 

Open the cloned directoy in `vscode` then:
    `mkdocs new .`
    `pip install mkdocs-material`

## Set Up Blog

- If you have not done so already, create a project for your blog, then edit the `mkdocs.yml` file to make sure it has the following content:


    `site_name:`example blog
    `site_description:`an example blog
    `site_url:` http://www.example.com


- The blog plugin will create a directory structure for your blog posts if it does not exist, so simply run `mkdocs serve` will create the structure.

Directory structure

````
  docs
      blog
          index.md
           posts
               index.md
````

Create a file `docs/blog/posts/myfirst.md` with the following contents:
    
````
---
date:
    created: 2023-12-31
---
```

## First-Level Heading

The blog plugin automatically creates navigation elements for the blog. The index page shows only the extract. When you select the "Continue
reading" link, you will get to the full blog post. Note how it has a URL generated from the first-level heading.



## Footnotes

[^1]: [Visual Studio](https://code.visualstudio.com)

[^2]: [Marked 2](https://marked2app.com)

[^3]: [Materials Mkdocs](https://squidfunk.github.io/mkdocs-material/)

[^4]: [GitHub](https://github.com)

[^5]: [Material for MkDocs Basic Blog Tutorial](https://squidfunk.github.io/mkdocs-material/tutorials/blogs/basic/?h=blog)

[^6]: [Material for MkDocs Documentation](https://squidfunk.github.io/mkdocs-material/)

Markdown Preview Enhanced