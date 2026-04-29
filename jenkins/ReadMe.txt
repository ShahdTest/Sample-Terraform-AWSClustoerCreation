Pipeline Stages:

Start of Pipeline: Initiates the pipeline execution.

Git Checkout: Clones the remote Git repository to retrieve the latest code.

Install Dependencies: Runs npm install to install project dependencies.

Test: Executes tests using npm test to ensure code quality.

Image Scan (Trivy): Scans the Docker image for vulnerabilities.

SonarQube Analysis: Analyzes code quality and detects issues.

Quality Gate: Checks if the code meets quality standards.

Build Docker Image: Builds a Docker image and tags it as sabdulaq/aul:devops.

Docker Image Scan: Scans the built Docker image for vulnerabilities.

Push Docker Image: Pushes the Docker image to the Docker registry.

Deploy Kubernetes Resources: Applies Kubernetes configurations (secrets, deployments, services, etc.).

Verify the Deployment: Checks the status of deployed pods to ensure they are running.

End of Pipeline: Marks the completion of the pipeline.