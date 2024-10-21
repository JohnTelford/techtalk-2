---
date: 2024-10-20
---

# Install -`material mkdocs`

October 16, 2024

> HTML created using `Draft` and `Marked 2` Steaming Preview

## Environment 

- Create new `GitHub` Repo
- `git clone` - new repo

Set up Python vertual environment

- `python -m venv venv`
-  `source venv/bin/activate`

Install `material mkdocs`:

Open the cloned directoy in `vscode`
- `mkdocs new .`
-  `pip install mkdocs-material`

## Set Up Blog

- If you have not done so already, create a project for your blog, then edit the `mkdocs.yml` file to make sure if has the following content:


    `site_name:` Blog Tutorial
    `site_description:` an example blog set up following the tutorial
    `site_url:` http://www.example.com


- The blog plugin will create a directory structure for your blog posts if it does not exist, so simply run `mkdocs serve` to get


```
   docs
    blog
       index.md
       posts
           index.md```

Create a file `docs/blog/posts/myfirst.md` with the following contents:
    

````
---
date:
    created: 2023-12-31
---```
`
## First-Level Heading

The blog plugin automatically creates navigation elements for the blog. The index page shows only the extract. When you select the "Continue
reading" link, you will get to the full blog post. Note how it has a URL generated from the first-level heading.