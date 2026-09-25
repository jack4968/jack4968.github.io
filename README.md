# jack4968.github.io

This repository contains the source files for my personal Quarto website. The website includes blog posts and computational analyses written in both Python and R.

## Requirements

To build the website, you will need:

- Quarto
- Python 3.14
- uv
- R 4.6
- renv

## Building the website

First, clone the repo and move into the project folder in git bash:

git clone  https://github.com/jack4968/jack4968.github.io.git
cd jack4968.github.io

Set up the Python environment with git bash by running:
uv sync

For the R environment, open R from the project folder and run:
renv::restore()

Once the environments are set up, render the website from the project folder in git bash with:

uv run quarto render

The rendered website will be in the `docs/` folder.
To preview the website locally, run in git bash:

uv run quarto preview
## Data

For my R and Python computational posts, I used the Palmer Penguins dataset.

The dataset can be found here: https://allisonhorst.github.io/palmerpenguins/

The Palmer Penguins data are available under a CC0 license. The data are included through the `palmerpenguins` packages, so no API key or login is needed to render the posts.