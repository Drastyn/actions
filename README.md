# Source Code Analysis Workflow

This repository includes a GitHub Actions workflow for performing source code analysis using SonarCloud.

## Workflow Configuration

The source code analysis workflow is defined in the `.github/workflows/source-code-analysis.yml` file. It includes the following steps:

1. Check out the repository
2. Set the Sonar branch
3. Run the SonarCloud GitHub Action for code analysis

## Setting Up Secrets

To use the source code analysis workflow, you need to set up the following secrets in your GitHub repository:

- `GITHUB_TOKEN`: This token is automatically provided by GitHub and does not require any additional setup.
- `SONAR_TOKEN`: This token is required for authenticating with SonarCloud. You can generate a new token in your SonarCloud account and add it as a secret in your GitHub repository.

To add a secret to your GitHub repository, follow these steps:

1. Go to the repository on GitHub.
2. Click on the "Settings" tab.
3. In the left sidebar, click on "Secrets and variables" and then "Actions".
4. Click the "New repository secret" button.
5. Enter the name of the secret (`SONAR_TOKEN`) and its value.
6. Click the "Add secret" button.

Once the secrets are set up, the source code analysis workflow will be able to authenticate with SonarCloud and perform code analysis on your repository.
