# SiteSurveyor

SiteSurveyor is an open-source land surveying software developed by Eineva Inc. Designed specifically for regions with limited internet connectivity, SiteSurveyor provides offline functionality, secure data storage, and automated processing for professional surveyors, government agencies, and educational institutions. Supported on mobile (iOS and Android), desktop, and web platforms, SiteSurveyor makes surveying more accessible, efficient, and accurate.

## Table of Contents
- [Features](#features)
- [Getting Started](#getting-started)
- [Installation](#installation)
- [Usage](#usage)
- [Branching Strategy](#branching-strategy)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Features
- **Cross-Platform Support**: Compatible with Android, iOS, desktop, and web.
- **Offline Capability**: Collect and store data offline with auto-sync once reconnected to the internet.
- **Automated Data Processing**: Automated calculations for slope, volume, elevation, and more.
- **Secure Data Management**: Data encryption, role-based access, and secure cloud storage.
- **Multi-Format Export**: Export reports in PDF, CSV, DXF, and DWG formats.
- **Collaborative Development**: Contributions from surveyors and developers worldwide.

## Getting Started
These instructions will help you get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites
- **Node.js** (for frontend and mobile development)
- **Python** (for backend development)
- **PostgreSQL** (database)
- **Git**

### Installation

#### Backend (Django)
1. Clone the repository:
   ```bash
   git clone https://github.com/YourUsername/SiteSurveyor.git
   cd SiteSurveyor/backend
   ```
2. Install Python dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Configure the PostgreSQL database (update credentials in `settings.py`), then migrate:
   ```bash
   python manage.py migrate
   ```
4. Run the server:
   ```bash
   python manage.py runserver
   ```

#### Frontend (React)
1. Navigate to the frontend directory:
   ```bash
   cd ../frontend
   ```
2. Install dependencies and start the development server:
   ```bash
   npm install
   npm start
   ```

#### Mobile (React Native)
1. Navigate to the mobile directory:
   ```bash
   cd ../mobile
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the mobile app:
   ```bash
   npm run start
   ```

## Usage
- **Desktop/Web**: Navigate to the frontend URL displayed in the terminal after running the frontend server.
- **Mobile**: Use the Expo Go app (for development) to scan the QR code generated after starting the mobile app.
- **Backend API**: Visit `http://127.0.0.1:8000` to access the Django backend API.

For more detailed usage instructions, please refer to the User Guide in the `docs` folder.

## Branching Strategy
SiteSurveyor follows a structured branching strategy to manage development and releases effectively:

- **`main`**: Holds the stable, production-ready code.
- **`develop`**: Contains the latest development code. All feature and bugfix branches are merged here.
- **`release`**: Used temporarily for preparing a new release. This branch is merged into both `main` and `develop` once the release is complete.
- **Feature branches** (`feature/your-feature-name`): Created from `develop` for new features.
- **Bugfix branches** (`bugfix/your-bugfix-name`): Created from `develop` to address issues found during development.
- **Hotfix branches** (`hotfix/your-hotfix-name`): Created from `main` for urgent fixes in production, merged into both `main` and `develop` after testing.

## Technologies Used
- **Backend**: Django, Django REST Framework, PostgreSQL
- **Frontend**: React, Redux, Axios
- **Mobile**: React Native, Watermelon DB (for offline data)
- **Data Synchronization**: Watermelon DB, PostgreSQL
- **Security**: Data encryption, user authentication

## Contributing
We welcome contributions from developers and surveyors! To contribute:

1. Fork the repository.
2. Create a new branch for your feature (e.g., `feature/your-feature-name`).
3. Make your changes, following coding standards.
4. Submit a pull request to the `develop` branch.

For detailed guidelines, please see our [CONTRIBUTING.md](./CONTRIBUTING.md) file.

## License
This project is licensed under the Mozilla Public License 2.0 - see the [LICENSE](./LICENSE) file for details.

## Contact
Eineva Inc.  
Email: [admin@eineva.co.zw](mailto:admin@eineva.co.zw)  
Website: [https://eineva.co.zw](https://eineva.co.zw)

For questions or feedback, please open an issue or contact us directly.

---

Thank you for being part of the SiteSurveyor community!
```
