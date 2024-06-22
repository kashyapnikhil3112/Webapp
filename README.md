# Webapp - Python
This GitHub Actions workflow automates the deployment of a Python application to an Azure Web App. 

Trigger: Runs on every push to the main branch.
Permissions: Grants necessary permissions for ID token writing and repository content reading.
Job (deploy): Executes on the latest Ubuntu environment.
Steps:
Checkout: Checks out the repository code.
Set up Python: Configures Python 3.8 environment.
Install dependencies: Installs the required Python packages from requirements.txt.
Azure Login: Authenticates to Azure using service principal credentials stored in GitHub Secrets.
Deploy to Azure: Uploads the application code to the specified Azure Web App using the publish profile.
In essence, this workflow ensures that every code push to the main branch results in an automated build and deployment of the application to Azure.
