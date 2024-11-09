# Contributing to SiteSurveyor

First of all, thank you for your interest in contributing to SiteSurveyor! We’re excited to collaborate with you to make land surveying software more accessible and effective. SiteSurveyor is open to contributions from developers, surveyors, and anyone interested in enhancing this tool.

## How to Contribute

### 1. Reporting Bugs or Requesting Features
- **Search Existing Issues**: Before creating a new issue, check to see if someone else has reported it.
- **Open a New Issue**: If no issue exists, feel free to create a new one! Please be as detailed as possible, including steps to reproduce the issue, screenshots if relevant, and suggested solutions if any.
- **Label Appropriately**: When creating an issue, use labels like `bug`, `enhancement`, or `documentation` to help us prioritize and organize.

### 2. Code Contributions

#### Prerequisites
- **Development Environment**: Ensure you have Node.js, Python, PostgreSQL, and Git installed.
- **Fork the Repository**: Create a fork of the main repository to work in your own branch.
- **Clone Your Fork**:
  ```bash
  git clone https://github.com/YourUsername/SiteSurveyor.git
  cd SiteSurveyor
  ```

#### Branching
- Create a new branch for your work. Use descriptive names for your branches:
  ```bash
  git checkout -b feature/your-feature-name
  ```

#### Setting up the Project
1. **Backend Setup (Django)**:
   - Install Python dependencies:
     ```bash
     cd backend
     pip install -r requirements.txt
     ```
   - Configure the PostgreSQL database in `settings.py`, then migrate:
     ```bash
     python manage.py migrate
     ```
   - Start the server:
     ```bash
     python manage.py runserver
     ```

2. **Frontend Setup (React)**:
   - Navigate to the frontend folder and install dependencies:
     ```bash
     cd ../frontend
     npm install
     ```
   - Start the development server:
     ```bash
     npm start
     ```

3. **Mobile Setup (React Native)**:
   - Navigate to the mobile directory, install dependencies, and start the mobile app:
     ```bash
     cd ../mobile
     npm install
     npm run start
     ```

#### Making Changes
- **Coding Standards**: Follow PEP8 for Python code and Airbnb's JavaScript style guide for JavaScript/React code.
- **Write Tests**: Ensure your changes are covered by tests. We use Django’s built-in testing for the backend and Jest for the frontend. Make sure all tests pass before submitting.
- **Commit Messages**: Write clear, concise commit messages describing your changes. Example:
  ```
  git commit -m "Add offline sync capability for mobile app"
  ```

### 3. Submitting Your Changes

1. **Push to Your Branch**:
   ```bash
   git push origin feature/your-feature-name
   ```
2. **Open a Pull Request**:
   - Go to the repository on GitHub and open a pull request from your branch.
   - In the pull request description, clearly explain the changes, why they’re needed, and any relevant issue numbers.
   - Mark the pull request with appropriate labels, such as `enhancement`, `bugfix`, or `documentation`.

3. **Address Review Feedback**:
   - A project maintainer will review your code. Please be responsive to feedback and make requested changes promptly.

### 4. Code of Conduct
All contributors must adhere to the [Code of Conduct](./CODE_OF_CONDUCT.md). Please respect fellow contributors and maintain a friendly, inclusive environment.

### 5. Contributor License Agreement (CLA)
To keep SiteSurveyor open-source, all contributors must agree to a Contributor License Agreement. You may be asked to sign a CLA before your pull request is merged.

## Getting Help
If you need any help, feel free to reach out by opening an issue or by emailing us at [admin@eineva.co.zw](mailto:admin@eineva.co.zw).

Thank you for helping make SiteSurveyor better for everyone!
```
