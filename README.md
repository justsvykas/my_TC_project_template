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
# Analysis

What is the main goal? What data are we using?

- Main findings in analysis

# Installation
This analysis is structured to be easily continued by another developer, with dependency management handled via the Poetry library. It follows consistent coding standards, enforced using Ruff for linting and the pre-commit library. To further ease distribution, this project is packaged for ease of use.

After placing yourself in your desired directory, run this command in your terminal to copy this repo.
```bash
git clone my_repo_url
```
Go to project directory.
```bash
cd my_dir/
```
## Windows
1. **Create a virtual environment:**
   ```powershell
   python -m venv venv
   ```
2. **Activate venv in PowerShell**
    ```powershell
    .\venv\Scripts\Activate.ps1
    ```
    **Alternatively in Command Prompt**
    ```
    venv\Scripts\activate.bat
    ```
3. **Install project_name package**
   ```powershell
   pip install .
   ```

## MacOS/Linux

1. **Create a virtual environment:**
   ```bash
   python3 -m venv venv
   ```
2. **Activate venv in PowerShell**
   ```bash
   source venv/bin/activate
   ```
3. **Install project_name package**
   ```bash
   pip install .
   ```

# Usage

Go to directory
```bash
cd src/project_name/
```
Open main analysis file
```bash
code main.ipynb
```
Run the notebook cells sequentially or review the precomputed outputs.

# Dependencies

- Python 3.12
- pip

For managing Python versions consider using [pyenv](https://github.com/pyenv/pyenv).

# Structure

```bash
.
├── ___.md                        # Documentation file for the task given by TC
├── .gitignore                    # Specifies files to ignore in Git version control
├── .pre-commit-config.yaml       # Configuration for pre-commit hooks
├── README.md                     # Project documentation
├── pyproject.toml                # Python project configuration (Poetry)
├── ruff.toml                     # Formatter and linter configuration (Ruff)
├── src                           # Source code directory
│    └── project_name             # Package directory
│       ├── __init__.py               # Marks this directory as a package
│       ├── main.ipynb                # Main file
│       └── utils                     # Directory for utility files
│           ├── __init__.py
│           ├── logs.py               # File contains functions for logging
│           ├── data_processing.py    # File contains functions to process data
│           └── plots.py              # File contains plot functions
├── tests                         # Directory for test cases
│   └── .gitkeep
└── .vscode                       # Directory for VS-specific settings
    ├── extensions.json           # Recommended VS Code extensions
    └── settings.json             # VS Code workspace settings
```

# Aknowledgments
