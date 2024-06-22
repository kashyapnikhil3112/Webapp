# Webapp - Python

**Name: azure-webaapps-python.yml**
This GitHub Actions workflow automates the deployment of a Python application to an Azure Web App. 

**Trigger**: Runs on every push to the main branch.
**Permissions**: Grants necessary permissions for ID token writing and repository content reading.
**Job (deploy):** Executes on the latest Ubuntu environment.
**Steps:**
**Checkout:** Checks out the repository code.
**Set up Python:** Configures Python 3.8 environment.
**Install dependencies:** Installs the required Python packages from requirements.txt.
**Azure Login:** Authenticates to Azure using service principal credentials stored in GitHub Secrets.
**Deploy to Azure:** Uploads the application code to the specified Azure Web App using the publish profile.

In essence, this workflow ensures that every code push to the main branch results in an automated build and deployment of the application to Azure.



**Name: Grant Write Permission**
Trigger: Runs on every pull request (on: pull_request: {}).
Job (dummy_job): Executes on the latest Ubuntu environment.
Steps:
Checkout: Checks out the repository code using the specified action (actions/checkout@v3).
Summary
This simple workflow is designed to run on pull request events. It doesn't perform any significant actions other than checking out the code, but it establishes a structure that can be expanded with additional steps as needed.
