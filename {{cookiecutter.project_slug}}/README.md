
[![Project Status](https://img.shields.io/badge/status-under%20development-yellow)](https://github.com/{{cookiecutter.github_repo_name}})


# {{cookiecutter.project_slug}}


**What is included on this project?**

📦 A basic `pyproject.toml` file to provide installation, packaging and distribution for your project.

🧪 Testing structure using [Pytest](https://docs.pytest.org/en/latest/).

✅ Code linter and code formatter [Ruff](https://github.com/charliermarsh/ruff).

🤝 Typing checking using [Mypy](https://mypy.readthedocs.io/en/stable/).

🔄 Continuous integration using [Github Actions](https://github.com/{{cookiecutter.github_repo_name}}/blob/main/.github/workflows) with jobs to check the quality of your code.

📃 Documentation with [Sphinx](https://www.sphinx-doc.org/en/master/) and [Readthedocs](https://readthedocs.org/).


## How to use this project ?

We use UV to manage the project virtual environment. UV is a single tool to replace pip, pip-tools, pipx, poetry, pyenv, twine, virtualenv. See the [official documentation](https://docs.astral.sh/uv/getting-started/installation/) for installation on your machine. 


Once installed, just run the following command to create the virtual environment and install the project dependencies:


```bash
uv sync 
```

or 

```bash
uv sync --dev
```

Quality control tools can be run as follows:

```bash
uvx ruff
```

```bash
uvx mypy
```

```bash
uv run pytest
```






## Project structure


This repository contains the following files and folders:

```
📦 Repository
 ┣ 📁 .github : contain the github settings
 ┃ ┗  📁 ISSUE_TEMPLATE : contains issues templates
 ┃    ┗ 📜 *.yaml
 ┃ ┗  📁 workflows : contains CICD processes
 ┃    ┣ 📜 code_quality.yml : Ruff + Black + mypy
 ┃    ┗ 📜 tests.yml : pytest + CodeCov
 ┣ 📁 docs: contains the documentation.
 ┣ 📁 project_name: contains the project code.
 ┃ ┗ 📜 *.py
 ┣ 📁 test: contains the project tests.
 ┃ ┗ 📜 test_*.py
 ┣ 📜 .gitignore: lists the files/folders to ignore for git.
 ┣ 📜 pre-commit-config.yaml: configuration file for pre-commit.
 ┣ 📜 CITATION.cff: citation information.
 ┣ 📜 CODE_OF_CONDUCT.md: code of conduct.
 ┣ 📜 CONTRIBUTING.md: contributing guidelines.
 ┣ 📜 LICENSE: license file.
 ┣ 📜 pyproject.toml: project configuration file.
 ┣ 📜 README.md: markdown file containing the project's readme.
 ┣ 📜 readthedocs.yml: Settings for readthedocs.
 ```

