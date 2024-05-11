# GitHub Actions Workflows for React and JavaScript Testing

This repository contains GitHub Actions workflows designed to automate building, testing, and ensuring the quality of a React application and its associated JavaScript code. Below you will find details about each workflow and how they contribute to the development process.

## Workflows

### 1. Build and Test React Application

**File**: `.github/workflows/build_test_react.yml`

This workflow triggers on any push or pull request to the `main` branch. It is designed to ensure that the React application builds and passes all tests before changes are merged into the main branch. The workflow runs on the latest Ubuntu runner provided by GitHub and uses Node.js version 16.x.

#### Steps:
- **Checkout**: Fetches the latest code from the repository to the runner.
- **Setup Node.js**: Sets up the specified version of Node.js.
- **Dependencies and Testing**:
  - Installs all npm dependencies.
  - Builds the React application.
  - Runs tests to verify that everything is functioning as expected.

### 2. Run JavaScript Tests

**File**: `.github/workflows/javascript-tests.yml`

This workflow is triggered by any push action to the repository. It focuses solely on running JavaScript tests, ensuring that the JavaScript code meets all specified testing criteria. Similar to the first, this also uses the latest Ubuntu runner and Node.js version 16.x.

#### Steps:
- **Checkout**: Fetches the latest code from the repository to the runner.
- **Setup Node.js**: Sets up the specified version of Node.js.
- **Dependencies and Testing**:
  - Installs npm dependencies.
  - Executes tests specified within the npm scripts.

## Contributing

To contribute to this project, ensure you follow the guidelines below:
- Fork the repository.
- Create a new branch for each feature or improvement.
- Make your changes and test locally.
- Submit a pull request to the `main` branch.

Please make sure your code complies with the coding standards and passes all the existing tests before submitting a pull request.

## License

This project is licensed under [LICENSE-NAME]. See the `LICENSE` file for more details.

