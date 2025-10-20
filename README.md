# 🧠 Online Bookstore Flask Application
### CI/CD Workflow and Automated Testing Report
**Student Name:** Faduma Mohamed Nur
**Student Number:** 2418794
**Module:** Web Technologies – Software Testing & CI/CD
**University:** St Mary’s University, Twickenham
**Date:** October 2025

---

## 📘 Project Overview
This project focuses on the testing and continuous integration of a Python Flask web application that simulates an online bookstore.
The aim was to design automated tests, improve reliability, and implement a CI/CD pipeline using **GitHub Actions**.
Through this project, I learned how to apply software testing principles to detect bugs, ensure stability, and automate testing workflows that continuously validate new code changes.

The Online Bookstore allows users to browse books by category, add them to the cart, and complete checkout. My work involved verifying that all these features function correctly while improving the efficiency and structure of the codebase.

---

## 🔗 Repository Information
The original project codebase was provided by St Mary’s University through the following repository:
🔗 [https://github.com/liuc8/online-bookstore-final-assessment](https://github.com/liuc8/online-bookstore-final-assessment)

I used the project template from the university and continued development in my personal GitHub account, where I implemented all testing and CI/CD improvements:
🔗 [https://github.com/sahra90/online-bookstore-final-assessment](https://github.com/sahra90/online-bookstore-final-assessment)

All automated testing, debugging, and performance improvements were carried out independently as part of my coursework submission.

---

## 🧩 Objectives
The key objectives of this assessment were to:
1. Develop and execute automated test cases for the Online Bookstore Flask Application.
2. Integrate the test automation into a CI/CD workflow using **GitHub Actions**.
3. Detect and fix bugs or inefficiencies in the existing code.
4. Improve the performance, maintainability, and structure of the system.
5. Provide detailed documentation of all tests, CI/CD processes, and results.

---

## ⚙️ Technologies and Tools Used
- **Programming Language:** Python 3.9
- **Framework:** Flask 3.0.3
- **Testing Tool:** Pytest 7.0.1 & Pytest-cov 4.0.0
- **CI/CD Platform:** GitHub Actions
- **Version Control:** Git and GitHub (`sahra90`)
- **IDE:** Visual Studio Code
- **Environment:** Virtual Environment (venv)
- **Code Quality:** Flake8 linting

---

## 🧠 CI/CD Workflow Setup
Continuous Integration (CI) was configured using **GitHub Actions**.
A workflow file named `.github/workflows/ci.yml` was created to automatically run tests whenever code was pushed to the repository.

The workflow includes the following steps:
1. **Checkout Repository:** Retrieves the latest code from GitHub.
2. **Set Up Python:** Configures Python 3.9 environment with caching.
3. **Install Dependencies:** Installs all required packages from `requirements.txt` and flake8.
4. **Set Environment Variables:** Configures Flask app settings and Python path.
5. **Lint with Flake8:** Checks code quality and syntax errors.
6. **Validate Flask Application:** Ensures the app can be imported successfully.
7. **Debug Test Discovery:** Shows test environment and discovered test files.
8. **Run Automated Tests:** Executes all Pytest cases with coverage reporting.

This automation ensures every commit triggers a full round of testing, improving feedback speed and code reliability.

📸 *Figure 1: Screenshot of the CI/CD pipeline configuration and successful GitHub Actions workflow run.*

---

## 🧪 Test Case Design and Coverage
Automated testing was carried out using **Pytest**, focusing on both functional and integration levels.
Each test case targeted a specific part of the application to ensure all features work as intended.

Examples of implemented tests include:
- **Homepage Route Test:** Verifies that the homepage loads correctly and displays book titles.
- **Category Filter Test:** Checks that `/books?category=Fiction` returns the correct filtered results.
- **Add-to-Cart Test:** Ensures users can add books to their cart successfully.
- **Cart Page Test:** Validates that the cart view loads with a 200 OK response.

All test files were stored inside the `test/` directory and executed via the command:
```bash
pytest -v --cov=. --cov-report=term-missing
```

### 📊 Test Results Summary
- **Total Tests:** 4 test cases
- **Test Status:** ✅ All tests passing (4/4)
- **Code Coverage:** 49% (157/310 lines covered)
- **Test Files:**
  - `test/test_cart.py` - Cart functionality tests
  - `test/test_categories.py` - Category and homepage tests
  - `test/conftest.py` - Test configuration and fixtures

### 🔧 Key Test Cases Implemented:
1. **`test_add_to_cart`** - Validates adding books to shopping cart
2. **`test_cart_page_loads`** - Ensures cart page renders correctly
3. **`test_homepage_displays_books`** - Verifies homepage book display
4. **`test_browse_category_fiction`** - Tests category filtering functionality

---

## 🐛 Bugs Found and Fixed
During the testing and CI/CD implementation process, several critical issues were identified and resolved:

### 1. **CI/CD Workflow Issues**
- **Problem:** Test discovery failure (exit code 5) - pytest couldn't find test files
- **Solution:** Added `pytest.ini` configuration and proper `PYTHONPATH` environment variable
- **Impact:** Enabled successful automated testing in GitHub Actions

### 2. **YAML Indentation Errors**
- **Problem:** GitHub Actions workflow had incorrect YAML indentation
- **Solution:** Fixed step indentation and list formatting in `.github/workflows/ci.yml`
- **Impact:** Workflow now runs without syntax errors

### 3. **Flask Environment Configuration**
- **Problem:** Flask app couldn't be imported during testing
- **Solution:** Added proper environment variables (`FLASK_APP`, `FLASK_ENV`, `PYTHONPATH`)
- **Impact:** Tests can now properly import and test the Flask application

---

## 🚀 Performance Improvements
1. **Dependency Caching:** Added pip dependency caching to speed up CI builds
2. **Test Organization:** Structured tests with proper fixtures and configuration
3. **Code Quality:** Integrated flake8 linting to maintain code standards
4. **Error Handling:** Added comprehensive error detection and reporting

---

## 📈 Results and Conclusion
This project successfully demonstrates the implementation of a comprehensive CI/CD pipeline for a Flask web application. Key achievements include:

- ✅ **100% Test Success Rate:** All 4 automated tests pass consistently
- ✅ **Automated CI/CD:** GitHub Actions workflow runs on every push/pull request
- ✅ **Code Quality Assurance:** Integrated linting and syntax error detection
- ✅ **Bug Resolution:** Fixed critical test discovery and environment issues
- ✅ **Documentation:** Comprehensive documentation of processes and results

The project demonstrates practical application of software testing principles and modern DevOps practices, contributing to more reliable and maintainable software development workflows.

---

## 🧾 Academic Information
**Student Name:** Faduma Mohamed Nur
**Student Number:** 2418794
**Module:** Web Technologies – Software Testing and CI/CD
**University:** St Mary’s University, Twickenham
**Date:** October 2025

---

## 💭 Reflective Notes
This project was developed as part of my MSc coursework to apply and demonstrate real-world software testing and CI/CD principles.
Through this task, I gained hands-on experience with automated testing, GitHub Actions, and workflow integration, learning how continuous integration helps maintain reliable code quality.
It also helped me understand how testing and automation play a key role in modern software engineering practices, improving efficiency and collaboration.

---

## 🕒 Last Updated
**Updated:** October 20, 2025 - CI/CD Pipeline Successfully Implemented
# Updated Sun Oct 20 22:56:06 JST 2025

