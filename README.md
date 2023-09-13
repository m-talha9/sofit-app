**DevOps Engineer Task for Sofit Consultancy**

I have already implemented a GitHub Actions pipeline in YAML for your HTML and JavaScript web application. The pipeline deploys the application to the Azure Web App Service, and I've passed a secret value from GitHub Secrets and displayed it on the index page.

- What triggers a deployment?

I have configured triggers for the CI/CD pipeline to activate on both commits and pull requests specifically for the main branch.

- How is the app packaged?

The steps and tools for packaging a web application can differ based on the technology stack and build process in use. In my case, where I have deployed an HTML and JavaScript application, I have streamlined the process to include these steps: Source Code, Configuration of Secret Value, Versioning, and Packaging.

- How is the app deployed (underlying infrastructure)

I have Deployed the application on Azure Web App Service.

- How is deployment versioned?

I have implemented auto-versioning for easier version management, and the current version is displayed on the index page. Versions will be managed through date wise. 

- How would you connect to the deployment?

I have generated a Personal Access Token (PAT) from Azure and securely stored it in the GitHub repository's secrets. In the CI/CD pipeline configuration, I simply referenced this secret variable to authenticate with Azure, making it easier to manage and protect sensitive authentication information.

- Add a sanity check to verify deployment worked well?

I have configured a sanity check in the CI/CD pipeline to verify the deployment status. If the check receives a 200 response, it displays a successful message; otherwise, it displays a failed message. This ensures that your pipeline performs basic validation to ensure successful deployments.

- How the app can be monitored?

We will monitor this application using a variety of monitoring stacks including Application Insights, Grafana, Prometheus, and the ELK Stack.
