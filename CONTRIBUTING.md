# Contributing to SiteSurveyor

Thank you for your interest in contributing to SiteSurveyor! We’re excited to collaborate with developers, surveyors, and anyone passionate about enhancing land surveying technology. Please follow these guidelines to help keep the project organized and maintainable.

## Table of Contents
- [Code of Conduct](#code-of-conduct)
- [How to Contribute](#how-to-contribute)
- [Branching Strategy](#branching-strategy)
- [Setting Up Your Development Environment](#setting-up-your-development-environment)
- [Coding Standards](#coding-standards)
- [Submitting a Pull Request](#submitting-a-pull-request)
- [Contributor License Agreement](#contributor-license-agreement)
- [Getting Help](#getting-help)

## Code of Conduct
Please read and adhere to our [Code of Conduct](./CODE_OF_CONDUCT.md) to maintain a welcoming and respectful environment for all contributors.

## How to Contribute

### Reporting Issues
- **Search Existing Issues**: Before creating a new issue, check the existing issues to see if it’s already reported or being discussed.
- **Open a New Issue**: If you don’t find an existing issue, create a new one. Include a detailed description, screenshots, and, if possible, steps to reproduce the issue.
- **Label Appropriately**: Use labels like `bug`, `enhancement`, or `documentation` to help us categorize and prioritize issues.

### Suggesting Enhancements
If you have ideas to improve SiteSurveyor, feel free to open an issue with the label `enhancement`. Describe the feature and explain why it would be useful.

## Branching Strategy
SiteSurveyor uses a structured branching strategy to streamline development and releases.

- **`main`**: The production-ready branch with stable code. Only final releases are merged here.
- **`develop`**: The main development branch, containing the latest code ready for testing and integration.
- **`release`**: Used temporarily to prepare releases, branched from `develop` and merged into both `main` and `develop` after release.

Temporary branches include:
- **Feature branches** (`feature/your-feature-name`): For new features, branched from `develop`.
- **Bugfix branches** (`bugfix/your-bugfix-name`): For fixes in development, branched from `develop`.
- **Hotfix branches** (`hotfix/your-hotfix-name`): For urgent fixes in production, branched from `main` and merged into both `main` and `develop`.

## Setting Up Your Development Environment

1. **Fork and Clone the Repository**
   ```bash
   git clone https://github.com/YourUsername/SiteSurveyor.git
   cd SiteSurveyor
   ```

2. **Install Dependencies**:
   - Backend:
     ```bash
     cd backend
     pip install -r requirements.txt
     ```
   - Frontend:
     ```bash
     cd ../frontend
     npm install
     ```
   - Mobile:
     ```bash
     cd ../mobile
     npm install
     ```

3. **Database Setup**: Configure PostgreSQL settings in `backend/settings.py`, then run migrations:
   ```bash
   python manage.py migrate
   ```

4. **Run Development Servers**:
   - Backend (Django):
     ```bash
     python manage.py runserver
     ```
   - Frontend (React):
     ```bash
     npm start
     ```
   - Mobile (React Native):
     ```bash
     npm run start
     ```

## Coding Standards
- **Python**: Follow PEP 8 standards for Python code in the backend.
- **JavaScript**: Use Airbnb’s JavaScript style guide for frontend and mobile code.
- **Testing**: All code changes should include tests:
  - **Backend**: Use Django’s testing framework.
  - **Frontend and Mobile**: Use Jest for unit tests.

## Submitting a Pull Request
1. **Branch from `develop`**: Make sure to branch from `develop` and name your branch appropriately:
   ```bash
   git checkout -b feature/your-feature-name
   ```
2. **Make and Commit Changes**:
   - Write meaningful commit messages describing your changes.
   - Ensure that your code follows coding standards and that all tests pass.
   ```bash
   git commit -m "Add feature for offline sync"
   ```

3. **Push to Your Branch**:
   ```bash
   git push origin feature/your-feature-name
   ```

4. **Open a Pull Request**:
   - Go to your fork on GitHub and create a pull request to the `develop` branch.
   - In the description, provide a summary of your changes, any relevant issue numbers, and label the PR (`enhancement`, `bugfix`, etc.).

5. **Respond to Review**: A project maintainer will review your code. Please address any feedback in a timely manner.

## Contributor License Agreement
To contribute, you may be asked to sign a Contributor License Agreement (CLA), granting us permission to use your contributions in the project.

## Getting Help
If you need help, feel free to open an issue with the label `question` or reach out via [admin@eineva.co.zw](mailto:admin@eineva.co.zw).

Thank you for helping to make SiteSurveyor better!
```


### Key Sections
- **Branching Strategy**: Clarifies how contributors should use branches.
- **Setting Up Your Development Environment**: Provides setup instructions.
- **Coding Standards**: Ensures consistency in code style.
- **Pull Request Process**: Outlines the steps for creating a PR.
