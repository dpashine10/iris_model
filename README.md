# Iris Flower Classification

## Overview
This project uses a Decision Tree classifier to predict the species of Iris flowers using the built-in Iris dataset from scikit-learn.

## Technologies
- Python
- scikit-learn
- pytest
- uv
- Git and GitHub
- GitHub Actions

## Project Structure
```text
iris-ml-project/
├── src/
│   ├── __init__.py
│   └── model.py
├── tests/
│   └── test_model.py
├── docs/
├── .github/
│   └── workflows/
│       └── tests.yml
├── pyproject.toml
├── uv.lock
├── README.md
└── .gitignore
```

## Setup
Install uv if it is not already installed. Then install the project dependencies:

```bash
uv sync
```

## Run the Model
```bash
uv run python src/model.py
```

The script trains a Decision Tree, evaluates its accuracy, and prints predictions.

## Run Automated Tests
```bash
uv run python -m pytest -v
```

The automated tests verify model training, dataset dimensions, prediction labels, and model accuracy.

## Continuous Integration
GitHub Actions automatically installs the dependencies and runs the automated tests on pushes to the main branch and pull requests targeting main.

## Results
The initial local model run achieved 93% accuracy on 30 test samples. Results are reproducible with the configured random seed.

## Author
Divy

## Development Workflow

Changes are developed on feature branches, tested using
GitHub Actions, and merged into main through pull requests.
