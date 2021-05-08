# 1. Introduction

This is the repository holding the completed assessment code for Credit Kudos' Income prediction exercise.
As part of the exercise, a machine learning model had to be built to predict transactions highly likely to be income.

# 2. Setting Up Your Development Environment

All python packages are managed by [Poetry](https://python-poetry.org/) and declared using pyproject.toml and its associated lockfile, poetry.lock.

## 2.1. Setting up Poetry
To install poetry, open up a terminal and type:

```bash
curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python -
```

To enable Poetry command line completion, open a terminal and type:

### 2.1.1 For Zsh shell
```bash
poetry completions zsh > ~/.zfunc/_poetry
```

### 2.1.2 For Oh-My-Zsh shell
```bash
mkdir $ZSH_CUSTOM/plugins/poetry
poetry completions zsh > $ZSH_CUSTOM/plugins/poetry/_poetry
```

### 2.1.3 Using Poetry along Anaconda
If you are not already using anaconda as a package manager, you can pass directly to the next section. If you are using anaconda, please follow the quick instructions below so that the installation with Poetry will not create additional virtual environment in your already created anaconda virtual env:

Open a terminal and copy/paste the following lines:

```bash
brew install jq
CONDA_ENV_PATH=$(conda info --json | jq '.envs_dirs[0]')
poetry config virtualenvs.path $CONDA_ENV_PATH
poetry config virtualenvs.create 0
```

## 2.2 Installing all the dependencies

You are now ready to set up the project locally:

Clone the repo with the following line:

```bash
git clone https://github.com/Ali-Parandeh/credit-kudos
```

Go to cloned repo folder and then open up terminal, and create the virtual environment that will host all the dependencies:

```bash
poetry env use 3.8
```

Then activate your virtual environment with the following command:

```bash
poetry shell
```

Finally, install all the necessary package all at once with:

```bash
poetry install
```

### 2.2.1 Anaconda users

For Anaconda user, the instruction above slightly differ from above:

First, go to cloned repo folder and then open up terminal create a virtual environment like you usually do for any project. Below we create a virtual env called `credit-kudos`:

```bash
conda create -n credit-kudos python=3.8
```

Then activate it:

```bash
conda activate credit-kudos
```

You can use now Poetry to install the package directly:

```bash
poetry install
```

# 2.3 Optional Jupyter Lab Extensions

- @timkpaine/jupyterlab_miami_nights
- @aquirdturtle/collapsible_headings

To install use:

```bash
jupyter labextension install <extension-name>
```
