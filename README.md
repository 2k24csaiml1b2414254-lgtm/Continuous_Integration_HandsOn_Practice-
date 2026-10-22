# Continuous Integration Hands-On Practice ⚙️

A beginner-friendly project demonstrating Continuous Integration (CI) using GitHub Actions, pytest, and a Streamlit application.

## 📌 About the Project

This project demonstrates how automated testing can be integrated into a development workflow using GitHub Actions.

The application is a simple Power Calculator built with Streamlit. Users can enter an integer and view its square, cube, and fifth power.

A GitHub Actions workflow is configured to run automated tests when code is pushed to the `main` branch or when a pull request targets `main`.

## ✨ Features

- Interactive calculator built with Streamlit
- Square, cube, and fifth-power calculations
- Automated tests using pytest
- GitHub Actions workflow for Continuous Integration
- Automated test execution on pushes and pull requests

## 🛠️ Tech Stack

- **Language:** Python
- **Frontend:** Streamlit
- **Testing:** pytest
- **CI/CD Automation:** GitHub Actions
- **Version Control:** Git and GitHub

## 📁 Project Structure

```text
Continuous_Integration_HandsOn_Practice-/
├── .github/
│   └── workflows/
│       └── ciyaml
├── .gitignore
├── CI_Revision_Notes.txt
├── LICENSE
├── README.md
├── _test.py
└── app.py
```

## ⚙️ Prerequisites

- Python 3.9 or a compatible version
- Git
- A GitHub account

## 🚀 Run the Application Locally

### 1. Clone the repository

```bash
git clone https://github.com/2k24csaiml1b2414254-lgtm/Continuous_Integration_HandsOn_Practice-.git
cd Continuous_Integration_HandsOn_Practice-
```

### 2. Install dependencies

```bash
python -m pip install streamlit pytest
```

### 3. Start the Streamlit app

```bash
python -m streamlit run app.py
```

Streamlit will provide a local URL, usually:

http://localhost:8501

## 🧪 Run Automated Tests

Execute the tests locally using:

```bash
python -m pytest _test.py -v
```

The test file covers square, cube, fifth-power calculations, and invalid input behavior.

## ⚙️ GitHub Actions Workflow

The workflow is located in `.github/workflows/` and is configured to run on:

- Pushes to the `main` branch
- Pull requests targeting the `main` branch

The workflow checks out the repository, sets up Python, installs dependencies, and runs pytest.

To inspect the result:

1. Open the repository on GitHub.
2. Navigate to the **Actions** tab.
3. Select the CI workflow.
4. Review the latest run and test output.

A successful workflow run indicates that the configured CI checks passed for that run.

## 📚 Learning Outcomes

Through this project, I am practicing:

- Understanding Continuous Integration
- Writing automated tests using pytest
- Configuring GitHub Actions workflows
- Triggering automated checks on code changes
- Reviewing test results through GitHub Actions

## 📄 License

This project is licensed under the MIT License. See the `LICENSE` file for details.
