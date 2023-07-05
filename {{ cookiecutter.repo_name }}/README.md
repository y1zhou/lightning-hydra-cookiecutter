<div align="center">

# {{ cookiecutter.project_name }}

[![python](https://img.shields.io/badge/-Python{{ cookiecutter.python_version }}-blue?logo=python&logoColor=white)](https://github.com/pre-commit/pre-commit)
<a href="https://pytorch.org/get-started/locally/"><img alt="PyTorch" src="https://img.shields.io/badge/PyTorch-ee4c2c?logo=pytorch&logoColor=white"></a>
<a href="https://pytorchlightning.ai/"><img alt="Lightning" src="https://img.shields.io/badge/-Lightning-792ee5?logo=pytorchlightning&logoColor=white"></a>
<a href="https://hydra.cc/"><img alt="Config: Hydra" src="https://img.shields.io/badge/Config-Hydra-89b8cd"></a>
<a href="https://github.com/ashleve/lightning-hydra-template"><img alt="Template" src="https://img.shields.io/badge/-Lightning--Hydra--Template-017F2F?style=flat&logo=github&labelColor=gray"></a><br>

</div>

## Description

{{ cookiecutter.description }}

## Installation

#### Pip

```bash
# clone project
git clone {{ cookiecutter.repo_url }}
cd {{ cookiecutter.repo_name }}

# [OPTIONAL] create conda environment
conda create -n {{ cookiecutter.repo_name }} python={{ cookiecutter.python_version }}
conda activate {{ cookiecutter.repo_name }}

# install pytorch according to instructions
# https://pytorch.org/get-started/

# install requirements
pip install -r requirements.txt
```

#### Conda

```bash
# clone project
git clone {{ cookiecutter.repo_url }}
cd {{ cookiecutter.repo_name }}

# create conda environment and install dependencies
conda env create -f environment.yaml -n {{ cookiecutter.repo_name }}

# activate conda environment
conda activate {{ cookiecutter.repo_name }}
```

## How to run

Train model with default configuration

```bash
# train on CPU
python src/train.py trainer=cpu

# train on GPU
python src/train.py trainer=gpu
```

Train model with chosen experiment configuration from [configs/experiment/](configs/experiment/)

```bash
python src/train.py experiment=experiment_name.yaml
```

You can override any parameter from command line like this

```bash
python src/train.py trainer.max_epochs=20 data.batch_size=64
```

## Contributing

### Documentation

By default, the project uses [MkDocs](https://www.mkdocs.org/) for all documentation.
Use `mkdocs serve` to view the docs, or `mkdocs build` to build static HTML files.
The project also initializes [mkdocstrings](https://mkdocstrings.github.io/), which enables automatic documentation from sources.

### Code

This project uses [pre-commit](https://pre-commit.com/) for identifying simple issues in the code before it is pushed to the remote repository.
Install `pre-commit` and the git hook scripts with:

```bash
pip install pre-commit
pre-commit install
```

Now all the hooks defined in [the pre-commit config](.pre-commit-config.yaml) will be run automatically before commiting.
You can also manually run them on all files:

```bash
pre-commit run --all-files
```
