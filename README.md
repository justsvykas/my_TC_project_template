# Project Template

Here I keep all the files and structure of my projects to ease development process in Turing College

# Usage of template:

- clone this repo into your local machine
- clone submission repo to your favorite projects directory
- copy the contents of template into submission repo directory
   **for Linux/Mac:**
   ```bash
   rsync -av --progress /root/Turing_College/project_tamplate/ ./ --exclude='.git'
   ```
   **Note** User path might be different
- commit and push to submission repo

**Template below**
---

---
# Project Name

This project is analysis of something. Where I have used somehting to draw below picture.

![Main picture](image.png)
# Analysis

What is the main goal? What data are we using?

- Main findings in analysis

# Installation
Below is the process to install this project on your local machine. However, there is **main.html** file in the root of the project that can be used to view the analysis without installing the project.

This analysis is structured to be easily continued by another developer, with dependency management handled via the Poetry library. It follows consistent coding standards, enforced using Ruff for linting and the pre-commit library. To further ease distribution, this project is packaged for ease of use.

After placing yourself in your desired directory, run this command in your terminal to copy this repo.
```bash
git clone https://github.com/TuringCollegeSubmissions/jusvyka-DS.v3.2.1.5
```
Go to project directory.
```bash
cd jusvyka-DS.v3.2.1.5/
```
install package
```bash
poetry install
```

# Usage

Go to directory
```bash
cd src/mental_health/
```
Open main analysis file
```bash
code main.ipynb
```
Run the notebook cells sequentially or review the precomputed outputs. Notice when running the notebook code will query and store data in data/ directory with.

When commiting to the repository, pre-commit will run ruff and some basic tests to ensure the code is up to standard.

# Dependencies

- Python 3.12
- poetry

For managing Python versions consider using [pyenv](https://github.com/pyenv/pyenv).
For using poetry take a look at [poetry installation](https://python-poetry.org/docs/#installation).

# Structure

```bash
.
├── __-.md                        # Documentation file for the task given by TC
├── .gitignore                    # Specifies files to ignore in Git version control
├── .pre-commit-config.yaml       # Configuration for pre-commit hooks
├── README.md                     # Project documentation
├── main.html                     # HTML file for viewing analysis without installation
├── pyproject.toml                # Python project configuration (Poetry)
├── ruff.toml                     # Formatter and linter configuration (Ruff)
├── src                           # Source code directory
│    └── project_name             # Package directory
│       ├── __init__.py          # Marks this directory as a package
│       ├── main.ipynb           # Main analysis notebook
│       └── utils/               # Directory for utility files
│           ├── __init__.py
│           ├── data_processing.py    # Data processing utilities
│           ├── logs.py              # Logging utilities
│           └── plots.py             # Visualization utilities
└── .vscode                       # Directory for VS-specific settings
    ├── extensions.json           # Recommended VS Code extensions
    └── settings.json             # VS Code workspace settings
```
# Aknowledgments
