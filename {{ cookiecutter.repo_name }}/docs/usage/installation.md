# Installation

```bash
# clone project
git clone {{ cookiecutter.repo_url }}
cd {{ cookiecutter.repo_name }}

# [OPTIONAL] create conda environment
conda create -n {{ cookiecutter.repo_name }} python={{ cookiecutter.python_version }}
conda activate {{ cookiecutter.repo_name }}

# install pytorch according to instructions
# https://pytorch.org/get-started/

# install requirements and the package in editable mode
pip install -e .
```
