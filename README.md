In this project, I set up a Jenkins pipeline for Continuous Integration (CI) and Continuous Deployment (CD) to automate the process of building and deploying an application. The goal was to create an efficient and automated pipeline that builds the application, runs tests, and deploys the app to a specified environment whenever new changes are pushed to the repository.

Here’s a breakdown of the steps I followed:
1. Setting Up Jenkins

    Installed Jenkins on an AWS EC2 instance (running Amazon Linux 2) to create the CI/CD pipeline.

    Configured Jenkins to work with Docker for containerization and deployment tasks.

2. Created a Jenkinsfile

    The Jenkinsfile defines the stages of the pipeline, including:

        Build: Compile and build the application Docker image.

        Test: Run automated tests (if any) to ensure the application is working as expected.

        Deploy: Deploy the application to a test environment or production server.

    I used Groovy scripting to define the pipeline in a Jenkinsfile stored in the project repository.

3. Configured Jenkins Pipeline

    Configured Jenkins to trigger the pipeline automatically on code commits using webhooks (from GitHub or GitLab).

    Set up Jenkins to pull the latest changes from the repository and start the pipeline process whenever there is a new commit.

4. Pipeline Stages

    The pipeline included several stages:

        Build Stage: Compiled and built the Docker image for the app.

        Test Stage: Ran any tests or validations to ensure the app was functioning properly.

        Deploy Stage: Deployed the application to a target environment (could be a staging or production environment).

5. Testing and Verification

    After configuring the Jenkinsfile, I tested the pipeline by pushing changes to the Git repository.

    I checked the Jenkins dashboard to verify that the pipeline triggered automatically and ran successfully through all the stages.

6. Pushed All Project Files to GitHub

    After completing the project, I pushed all the project files (Terraform and Jenkins configurations, along with the respective logs) to my existing GitHub repository:
    ➡️ elevatelabs_task2
