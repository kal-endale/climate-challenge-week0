# Climate Change Week 0

## Overview
This repository contains the setup for **Week 0**. This README explains how to reproduce the environment and verify the setup locally. GitHub Actions is also configured to run checks on every push to the `main` branch.

## Prerequisites
- Python 3.x
- Git

## 1) Clone the repository
```bash
git clone <repo-url>
cd climate-change-week0

2) Create and activate a Python virtual environment
Option A: venv (recommended)
macOS/Linux:

bash
python -m venv venv
source venv/bin/activate

Windows:

bash
python -m venv venv
venv\Scripts\activate

Option B: conda
bash
conda create -n climate-env python=3.x -y
conda activate climate-env

3) Install dependencies
With your environment activated:

bash
pip install -r requirements.txt

4) Run checks locally (if applicable)
This project uses GitHub Actions to run checks. If your coursework specifies a local command to run the same checks, run it here. (Replace the example command(s) below with the real ones from your assignment/CI workflow.)

Examples (edit as needed):

bash
python --version
# python -m pytest
# or: python your_script.py

Git hygiene notes
data/ is excluded via .gitignore so large files are not committed.
Jupyter notebook checkpoints (.ipynb_checkpoints/) are also ignored.
CI / GitHub Actions
A GitHub Actions workflow is located at:

./.github/workflows/ci.yml
It runs automatically on pushes to the main branch to verify the environment and checks.

