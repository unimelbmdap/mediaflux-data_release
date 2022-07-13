# Mediaflux-backed public data release template


## Usage

- [Fork this repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo).  
  After forking you can also change the name of the repository, if you wish, by going to `settings` -> `general` -> `repository name`. 

- [Enable github pages](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site) for your newly forked repo.  
  For step 4, choose the `gh-pages` branch.  
  You can skip step 5.

- Edit the `mkdocs.yml` file as needed, at the very least you will want to change the title.

- Edit the `docs/index.html` as needed.
  The template uses the [Material theme](https://squidfunk.github.io/mkdocs-material/) for [MkDocs](https://www.mkdocs.org). Details of the syntax and extensive formatting options can be found by checking out their sites.

- Commit and push your changes.

- Behind the scenes, a github action will run that will automatically generate your site!
  The result can be found (and is publically accessible) at `https://<username>.github.io/<repo-name>/`, where `<username>` and `<repo-name>` should be replaced appropriately.


## Development

If you wish to develop the site locally, you will require [Git](https://git-scm.com) and [Python (>v3.7)](https://www.python.org).

After cloning your fork locally and cd'ing into it, you can install the dev requirements using the following commands:

```sh
python -m pyenv ./.venv
source .venv/bin/activate
pip install -r requirements.txt
```

> ⚠️ **Note**
> If you close your terminal, you will need to do the `source .venv/bin/activate` step (only!) again to activate your Python virtual environment. You will not need to run the other two lines again though.

You can then serve the site locally using

```sh
mkdocs serve
```

When you modify either `mkdocs.yml` or any of the files in `docs/`, the locally served site will be automatically updated. Once you are happy with your changes, commit and push them to your github fork. This will then trigger the rebuild of the public facing site to match the new version of the site.
