# 🧠 Online Bookstore Flask Application
### CI/CD Automation and Software Testing

**Student Name:** Faduma Nur
**Student Number:** 2418794
**Module:** Web Technologies – Software Testing and CI/CD
**University:** St Mary's University, Twickenham
**Date:** October 2025

---

## 📘 Project Overview
This repository contains my implementation of automated testing and a Continuous Integration (CI) workflow for a Python Flask web application, developed as part of my MSc Web Technologies module.

The Online Bookstore Flask application allows users to browse books, view categories, add items to their cart, and complete checkout. The focus of this project was to apply **software testing methodologies** and **CI/CD automation** to ensure system reliability, quality, and performance.

The project aims to demonstrate professional testing and automation practices similar to those used in real-world software engineering.

---

## 🎯 Objectives
- Implement complete test coverage using **Pytest**
- Integrate continuous testing using **GitHub Actions (CI/CD)**
- Improve code efficiency and maintainability
- Apply linting and code quality checks using **Flake8**
- Document the testing process and CI/CD workflow

---

## ⚙️ Technologies and Tools Used
| Category | Tools / Technologies |
|-----------|----------------------|
| **Programming Language** | Python 3.9 |
| **Framework** | Flask |
| **Testing Framework** | Pytest, Pytest-cov |
| **Code Quality Tool** | Flake8 |
| **Automation Platform** | GitHub Actions |
| **Version Control** | Git and GitHub (`sahra90`) |
| **Editor** | Visual Studio Code |
| **OS** | macOS |

---

## 🔄 CI/CD Workflow
A workflow file named `.github/workflows/ci.yml` automates the testing pipeline.
It runs every time code is pushed to the **main** or **develop** branch, or when a pull request is opened.

### Workflow Steps
1. **Checkout Repository** – Retrieves the latest code from GitHub.
2. **Set Up Python** – Installs Python 3.9 on the runner environment.
3. **Cache Dependencies** – Reuses installed packages to speed up runs.
4. **Install Dependencies** – Installs all packages from `requirements.txt`.
5. **Run Flake8 Linting** – Checks for syntax errors and style issues.
6. **Validate Flask App** – Confirms that `app.py` runs correctly.
7. **Run Pytest** – Executes automated tests with coverage.
8. **Generate and Upload Coverage Report** – Produces coverage.xml and uploads results via Codecov.
9. **Summary** – Displays pipeline summary in the Actions log.

This workflow ensures continuous testing, quick feedback, and maintains project stability.

---

## 🧪 Test Case Design and Coverage
The **tests/** directory includes multiple automated test cases written in **Pytest**.
These tests verify both unit-level and integration-level behavior of the system, focusing on the main user interactions.

Key test cases include:
- `test_homepage()` – Ensures homepage loads correctly.
- `test_category_filter()` – Checks that category filtering returns the right books.
- `test_add_to_cart()` – Confirms that books are added correctly.
- `test_cart_page()` – Verifies that cart contents are displayed properly.

All tests were executed automatically through GitHub Actions.
The final coverage report achieved **49% coverage**, verifying that key routes and logic worked as expected.

---

## 📈 Results and Improvements
Integrating **CI/CD automation** reduced manual testing time and improved reliability.
Before automation, tests were run locally; after configuration, each commit automatically triggered the test suite.

### Key Improvements
- Early detection of route and YAML errors.
- Consistent validation of every commit.
- Enhanced code readability through Flake8 linting.
- Improved workflow speed with caching and parallel steps.

This automation mirrors real-world DevOps pipelines used in professional environments.

---

## 🧭 Repository Information
The base code was provided by **St Mary's University** via the official repository:
[University Source Repository](https://github.com/liuc8/online-bookstore-final-assessment)

I forked and configured it under my own GitHub profile **`sahra90`**, adding automated testing and CI/CD integration.

---

## 🪄 Learning Reflection
Working on this assessment strengthened my understanding of:
- Designing structured and reusable test cases.
- Debugging Python applications using test coverage feedback.
- Implementing CI/CD pipelines to improve collaboration and quality assurance.
- Applying industry-standard tools such as Pytest, Flake8, and GitHub Actions.

This experience helped me gain confidence in applying real-world automation practices that ensure continuous validation and deployment reliability.

---

## 🕓 Last Updated
**Updated:** October 20, 2025 - CI/CD Pipeline Verified ✅
