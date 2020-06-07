# Data Science Project Template

A template repository for data science projects.

The file organisation is losely based on [TDSP Project Structure](https://github.com/Azure/Azure-TDSP-ProjectTemplate) and [CookieCutter Data Science](https://github.com/drivendata/cookiecutter-data-science/).

## Using the template

This template requires Python 3 and [cookiecutter](https://cookiecutter.readthedocs.io/en/latest/installation.html).

1. Install [cookiecutter](https://cookiecutter.readthedocs.io/en/latest/installation.html).

   ```bash
   pip install cookiecutter jinja2_git
   ```
2. Create a new project:
   ```bash
   cookiecutter gh:sheikhomar/cookiecutter-data-science
   ```
3. Initialise a new Git repository:
   ```bash
   cd <NEW_PROJ_DIR>
   git init
   git add .
   git commit -m "Initial commit."
   git remote add origin <GIT_REMOTE_URL>
   git push -u origin master
   ```
4. Install [pyenv](https://github.com/pyenv/pyenv) and [Poetry](https://python-poetry.org/docs/) if not already installed:
   ```bash
   curl https://pyenv.run | bash
   pyenv install
   curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python
   source $HOME/.poetry/env
   ```
5. Install dependencies:
   ```bash
   poetry install
   ```
6. Install the pre-commit Git hooks:
   ```bash
   poetry run pre-commit install
   ```
