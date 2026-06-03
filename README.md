# OptiWell Docs

## Clone Repository

### HTTPS

```bash
git clone https://github.com/cyphercrescent/optiwelld.git
cd optiwell-docs
```


## Python Virtual Environment Setup

Use a project-local virtual environment named `.venv`.

### 1) Create the virtual environment

#### Linux and macOS

```bash
python3 -m venv .venv
```

#### Windows (PowerShell)

```powershell
py -m venv .venv
```

#### Windows (Command Prompt)

```bat
py -m venv .venv
```

### 2) Activate the virtual environment

#### Linux and macOS

```bash
source .venv/bin/activate
```

#### Windows (PowerShell)

```powershell
.venv\Scripts\Activate.ps1
```

#### Windows (Command Prompt)

```bat
.venv\Scripts\activate.bat
```

### 3) Install dependencies

```bash
python -m pip install --upgrade pip
pip install -e .
```

This installs all required packages declared in `pyproject.toml`.

### 4) Deactivate when done

```bash
deactivate
```

## Run Quarto

### 1) Activate the virtual environment

```bash
source .venv/bin/activate
```

### 2) Preview with live reload (recommended)

```bash
quarto preview
```

This builds the site, opens your browser to `http://localhost:3456`, and automatically rebuilds and refreshes when you save changes to any `.qmd` file.

### 3) One-time render (optional)

```bash
quarto render
```

Renders the site once to `_site/` and exits. Useful for CI/CD or final builds.

## Verify Remote Connection

Use these commands to confirm local auth and remote access:

```bash
gh auth status -h github.com
git remote -v
git ls-remote --heads origin
```
