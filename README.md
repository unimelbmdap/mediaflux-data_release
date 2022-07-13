Mediaflux-backed public data release template
=============================================

Usage
-----

- [Fork this repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo).
  After forking you can also change the name of the repository, if you wish, by going to `settings` -> `general` -> `repository name`. 

- [Enable github pages](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site) for your newly forked repo.
  For step 4, choose the `gh-pages` branch.
  You can skip step 5.

- Edit the `docs/index.html` for your needs.
  The template uses the [Material theme](https://squidfunk.github.io/mkdocs-material/) for [MkDocs](https://www.mkdocs.org). Details of the syntax and extensive formatting options can be found by checking out their sites.

- Commit and push your changes.

- Behind the scenes, a github action will run that will automatically generate your site.
  The result can be found (and is publically accessible) at `https://<username>.github.io/<repo-name>/`, where `<username>` and `<repo-name>` should be replaced appropriately.
