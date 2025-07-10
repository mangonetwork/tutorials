# MANGO User Guide

This is the repository hosting all the files used to create the MANGO User Guide, available at https://mangonetwork.github.io/tutorials

This is intended to be a basic guide to help scientific users get started with MANGO data.  It is available as a [jupyter book](https://jupyterbook.org/en/stable/intro.html) hosted on [GitHub Pages](https://pages.github.com/). The notebooks included provide examples of some of the more common analysis and plotting tasks.  Please feel free to download notebooks if they are useful, or copy/paste examples into your own code and modify as appropriate!

## Developing
Follow these steps to add or modify material in these tutorial guides.

1. Clone a local copy of this repository.
2. Install the current requirements in your environment.  This can be done from the environment file if you use conda.
```
conda env update --name <your_environment_name> --file environment.yml
```
If you typically install packages with pip, you can do this from `requirements.txt` instead.
```
pip install -r requirements.txt
```
3. Add your content.  This can be in the form of markdown files or jupyter notebooks.  All content files should be contained within the `src` directory and subdirectories within.
4. Add any pages you created to `_toc.yml`.
5. Add any packages your examples rely on to `environment.yml` and `requirements.txt`.  Try to avoid using large packages or anything that may have trouble with a default installation when possible.
6. Build the book locally.
```
jupyter-book build .
```
7. Check the local build to make sure your material looks correct.  The build command should have created the file `_build/html/index.html` which can be opened in any browser.
8. Commit your changes.  This can happen at multiple stages as you develop content.
9. Push changes to GitHub.  Any pushes to the `main` branch should update the webpage automatically, but it may take several minutes.

Refer to the [jupyter book docs](https://jupyterbook.org/en/stable/intro.html) for more detailed information about syntax and building the book.

