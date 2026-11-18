# Soccer Penalties Modelling Project

## 1. Project Overview

This project will explore soccer penalty kicks using data analysis, statistical techniques and machine learning.

The initial setup establishes a reproducible Python environment and an organised project structure for data preparation, exploratory analysis, modelling and reporting.

## 2. Development Environment

- **Operating system:** Windows
- **Code editor:** Visual Studio Code (VS Code)
- **Python:** 3.12.10
- **Virtual environment:** `.venv`
- **Version control:** Git
- **Remote repository:** GitHub (private repository)

## 3. Initial Setup — Steps Completed

### Step 1: Install the required software

Installed and verified the following:

- Python 3.12.10
- Git
- Visual Studio Code
- Python extension for VS Code

### Step 2: Create the project folder

Created the local project folder:

```text
C:\Users\micha\Python_Projects\pens_model_nov_26
```

Opened this folder in VS Code as the project workspace.

### Step 3: Initialise Git and connect GitHub

- Initialised a local Git repository.
- Set the default branch to `main`.
- Created a private GitHub repository named `pens_model_nov_26`.
- Connected the local repository to GitHub using the `origin` remote.
- Pushed the initial commit to GitHub.

Check the repository status using:

```powershell
git status
```

Check the remote connection using:

```powershell
git remote -v
```

### Step 4: Create the Python virtual environment

From the project root, created a virtual environment:

```powershell
python -m venv .venv
```

Activated it in the VS Code PowerShell terminal:

```powershell
.\.venv\Scripts\Activate.ps1
```

The terminal should show `(.venv)` at the beginning of the prompt.

Verified the active Python interpreter:

```powershell
python -c "import sys; print(sys.executable)"
```

Expected path:

```text
C:\Users\micha\Python_Projects\pens_model_nov_26\.venv\Scripts\python.exe
```

In VS Code, select this environment through **Ctrl+Shift+P → Python: Select Interpreter** if necessary.

### Step 5: Configure `.gitignore`

Created and configured `.gitignore` to exclude unnecessary or generated files, including:

- Virtual environments and Python cache files
- Secrets and local environment configuration
- Raw, processed and other generated datasets
- Trained model files and machine learning artefacts
- Logs, generated reports and temporary files
- Operating system and editor-specific files

Empty placeholder files named `.gitkeep` were added to selected data and model folders so Git can track those folders without tracking their contents.

### Step 6: Create the project structure

The project currently uses this structure:

```text
pens_model_nov_26/
├── data/
│   ├── raw/
│   │   └── .gitkeep
│   └── processed/
│       └── .gitkeep
├── models/
│   └── .gitkeep
├── notebooks/
├── reports/
├── src/
├── .venv/
├── .gitignore
├── README.md
└── requirements.txt
```

Folder purposes:

- `data/raw/` — original datasets, preserved without modification.
- `data/processed/` — cleaned and transformed datasets.
- `models/` — trained models and associated artefacts.
- `notebooks/` — interactive exploration, analysis and experiments.
- `reports/` — analysis outputs, charts, tables and summaries.
- `src/` — reusable Python source code.
- `.venv/` — isolated Python environment; excluded from Git.

Note: `.venv/` may not be visible in the VS Code Explorer if hidden or excluded from the displayed files.

### Step 7: Create `requirements.txt`

Added the initial Python dependencies:

```text
pandas
numpy
matplotlib
seaborn
scikit-learn
jupyter
```

These are used for:

- **pandas** — data manipulation and analysis.
- **numpy** — numerical calculations.
- **matplotlib** — charts and visualisations.
- **seaborn** — statistical visualisations.
- **scikit-learn** — machine learning and model evaluation.
- **jupyter** — interactive notebooks.

### Step 8: Install the dependencies

With `.venv` activated, ran:

```powershell
python -m pip install -r requirements.txt
```

The installation completed successfully.

### Step 9: Verify the libraries

Ran the following command:

```powershell
python -c "import pandas, numpy, matplotlib, seaborn, sklearn, jupyter; print('All six libraries imported successfully!')"
```

The imports succeeded, confirming that the initial dependencies are available in the active environment.

## 4. Getting Started in Future Sessions

When reopening this project:

1. Open the `pens_model_nov_26` folder in VS Code.
2. Open a new terminal using **Terminal → New Terminal**.
3. Activate the virtual environment:

   ```powershell
   .\.venv\Scripts\Activate.ps1
   ```

4. Confirm the active interpreter if needed:

   ```powershell
   python -c "import sys; print(sys.executable)"
   ```

5. If dependencies are missing, install them using:

   ```powershell
   python -m pip install -r requirements.txt
   ```

6. Check the Git working tree:

   ```powershell
   git status
   ```

If setting up a fresh local copy, clone the private GitHub repository first, open the cloned folder in VS Code, create `.venv`, and install the dependencies.

## 5. Git and Version Control Notes

- The local Git repository is connected to the private GitHub repository.
- The initial project commit has been pushed to the `main` branch.
- Subsequent setup changes are being grouped for a later, meaningful commit.
- Do not commit the `.venv` directory, secrets, large datasets or generated model files.
- Review `git status` before staging or committing changes.

## 6. Current Status

**Initial environment setup: complete.**

- [x] Python, Git and VS Code installed.
- [x] Git repository connected to GitHub.
- [x] Virtual environment created and verified.
- [x] `.gitignore` configured.
- [x] Initial project folders created.
- [x] `requirements.txt` populated.
- [x] Dependencies installed and import-tested.
- [ ] README updated with this setup documentation.
- [ ] Initial setup changes reviewed and committed together.

## 7. Planned Next Steps

1. Save this README documentation.
2. Review the setup files and Git status.
3. Create a small Python smoke-test script.
4. Decide on the data source and structure for the penalty dataset.
5. Begin exploratory data analysis.
6. Develop and evaluate suitable statistical or machine learning models.
7. Document results and limitations in reports.

