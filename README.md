# 🧬 Biohacking Personal Optimization Predictor

[![Project Status: Active](https://img.shields.io/badge/Project%20Status-Active-brightgreen)](https://shields.io/)
[![Build Status: Passing](https://img.shields.io/badge/Build-Passing-brightgreen)](https://shields.io/)
[![Code Style: Black](https://img.shields.io/badge/Code%20Style-Black-000000.svg)](https://black.readthedocs.io/en/stable/)
[![Linting: Ruff](https://img.shields.io/badge/Linting-Ruff-blue)](https://docs.astral.sh/ruff/)

---

<!-- TOC -->
<!-- TOC -->
## 📚 Table of Contents

- [🧬 Biohacking Personal Optimization Predictor](#-biohacking-personal-optimization-predictor)
  - [📚 Table of Contents](#-table-of-contents)
  - [Overview](#overview)
  - [Project Goals](#project-goals)
  - [Skills and Technologies Used](#skills-and-technologies-used)
  - [Code Quality and Style](#code-quality-and-style)
    - [How to Format Code](#how-to-format-code)
    - [How to Lint Code](#how-to-lint-code)
  - [All code should pass both Black formatting and Ruff linting before being committed.](#all-code-should-pass-both-black-formatting-and-ruff-linting-before-being-committed)
  - [Project Structure](#project-structure)
  - [Test-Driven Development Workflow](#test-driven-development-workflow)
  - [Dataset(s)](#datasets)
  - [How to Run the Project](#how-to-run-the-project)
    - [1. Clone the Repository](#1-clone-the-repository)
    - [2. Set Up the Virtual Environment](#2-set-up-the-virtual-environment)
    - [3. Install Required Packages](#3-install-required-packages)
    - [4. Running Tests](#4-running-tests)
    - [5. Running the Streamlit App (Potential for Later)](#5-running-the-streamlit-app-potential-for-later)
  - [License](#license)
  - [Acknowledgments](#acknowledgments)
  - [✨ Project Status](#-project-status)
  - [🛤️ Roadmap](#️-roadmap)
    - [Core Development](#core-development)
    - [Machine Learning](#machine-learning)
    - [Dashboard Development](#dashboard-development)
    - [Code Quality and Maintenance](#code-quality-and-maintenance)
<!-- /TOC -->

---
## Overview

This project builds a machine learning model that predicts personalized biohacking recommendations based on individual lifestyle data inputs (sleep patterns, workout intensity, supplement intake, screen time, etc.).  
It follows a **Test-Driven Development (TDD)** approach: writing tests first, then building the functionality to pass those tests.

---

## Project Goals

- Predict supplement regimens and habit optimizations based on user data.
- Visualize the relationships between health behaviors and biohacking goals.
- Build the project using a **Test-Driven Development** workflow to ensure reliability, maintainability, and professional-grade code quality.
- Deploy an interactive Streamlit dashboard for user inputs and predictions.

---

## Skills and Technologies Used

- **Programming Languages:** Python
- **Data Analysis:** Pandas, NumPy
- **Machine Learning:** Scikit-Learn
- **Testing Framework:** PyTest
- **Formatting Tool:** Black (auto-formatting Python code to PEP8 standards)
- **Linting Tool:** Ruff (fast Python linter and code quality checker)
- **Data Visualization:** Matplotlib, Seaborn
- **(Front-End):** Streamlit
- **Version Control:** Git, GitHub
- **Containerization:** Docker (for deployment)

---

## Code Quality and Style

This project follows professional Python code quality standards:

- **Formatting:** [Black](https://black.readthedocs.io/en/stable/) is used to automatically format all `.py` files.
- **Linting:** [Ruff](https://docs.astral.sh/ruff/) is used for ultra-fast linting and code quality checking.

### How to Format Code

Format all Python files in the project automatically:

```bash
black .
```

### How to Lint Code

Check all Python files for code quality issues:

```bash
ruff check .
```

Automatically fix certain linting issues:

```bash
ruff check . --fix
```

## All code should pass both Black formatting and Ruff linting before being committed.

## Project Structure

```
biohacking-optimizer/
│
├── data/                  # Datasets (raw and processed)
├── notebooks/             # Jupyter notebooks for EDA, modeling
├── scripts/               # Core functionality (cleaning, modeling)
├── tests/                 # Unit tests (TDD workflow)
├── models/                # Saved models (pickle files)
├── dashboard/             # Streamlit app (optional)
├── .gitignore             # Ignore venv/ and other unnecessary files
├── README.md              # Project overview
├── requirements.txt       # Python libraries needed
└── venv/                  # Local virtual environment (not pushed to GitHub)
```

---

## Test-Driven Development Workflow

- Define expected behavior for each function or module.
- Write unit tests inside `/tests/`.
- Write the actual code to pass those tests.
- Refactor while keeping all tests green.
- Run full test suite regularly using:
  ```bash
  pytest
  ```

---

## Dataset(s)

- [ ] Public health/lifestyle datasets (Kaggle, UCI ML Repo, PhysioNet)
- [ ] Potential: Personal health tracking data (exported from devices or medical logs).

---

## How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/biohacking-optimizer.git
cd biohacking-optimizer
```

### 2. Set Up the Virtual Environment

```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Required Packages

```bash
pip install -r requirements.txt
```

### 4. Running Tests

```bash
pytest
```

### 5. Running the Streamlit App (Potential for Later)

```bash
streamlit run dashboard/app.py
```

---

## License

This project is open-source and available under the [MIT License](LICENSE).

---

## Acknowledgments

- Open-source datasets and contributors.
- Inspiration from the biohacking, personal optimization, and data science communities.

---

## ✨ Project Status

> 🚀 Initial project setup complete.  
> ✅ Virtual environment configured and activated.  
> ✅ GitHub repository created, connected, and pushed with clean, organized commits.  
> ✅ Project structure established with clear separation between scripts and tests.  
> ✅ Pytest configured for Test-Driven Development (TDD) workflow.  
> ✅ Black configured for automatic code formatting (PEP8 compliance).  
> ✅ Ruff configured for fast code linting and quality checking.  
> ✅ VS Code fully integrated with Black (format on save) and Pytest (test discovery and running).
> ✅ Core data cleaning utilities development:
> - `drop_missing_rows(df)`
> - `drop_columns_with_many_nans(df, threshold=0.5)`
> - `drop_duplicate_rows(df)`
> - `fill_missing_with_mean(df, columns)`
> 
> 🎯 Currently preparing for Phase 2D:
> - Expanding feature coverage (e.g., median imputation, scaling, outlier handling)
> - Continuing TDD-style function development
> - Beginning dataset preparation and exploratory data analysis (EDA)

---

## 🛤️ Roadmap

The following milestones are planned to expand the Biohacking Personal Optimization Predictor project:

### Core Development
- [x] Set up virtual environment, GitHub repo, and project structure
- [x] Configure Pytest for Test-Driven Development (TDD)
- [x] Configure Black for code formatting and Ruff for linting
- [x] Build initial data cleaning utilities:
    - `drop_missing_rows`
    - `drop_columns_with_many_nans`
    - `drop_duplicate_rows`
    - `fill_missing_with_mean`
- [ ] Expand data cleaning functions (e.g., fill with median, handle outliers, standardize features)
- [ ] Expand unit tests for new utilities and data processing functions
- [ ] Start exploratory data analysis (EDA) on sample or personal dataset


### Machine Learning
- [ ] Build initial predictive model (e.g., recommend supplements or habits based on input features)
- [ ] Train and evaluate model performance
- [ ] Tune hyperparameters and feature engineering

### Dashboard Development 
- [ ] Develop basic Streamlit dashboard for user input and predictions
- [ ] Add visualizations for lifestyle data trends
- [ ] Deploy the app locally or publicly 

### Code Quality and Maintenance
- [ ] Maintain 100% passing unit tests
- [ ] Maintain formatting and linting standards across all code
- [ ] Update README and documentation as the project evolves

---

