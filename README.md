# Depolyment of Java based Application through CI/CD Jenkins pipeline using Maven,SonarQube, Docker, Argo CD, Helm and Kubernetes 

![Screenshot 2023-03-29 124201](https://user-images.githubusercontent.com/91549516/229478815-a58d95d6-9141-454d-8969-62a7b0d1ce30.png)

Here are the step-by-step details to set up an end-to-end Jenkins pipeline for a Java application using SonarQube, Argo CD, Helm, and Kubernetes:

Prerequisites:

   -  Java application code hosted on a Git repository
   -   Jenkins server
   -   Docker installed
   -  Kubernetes cluster
   -  Helm package manager
   -  Argo CD
   
   steps: 
   
     1. I have Installed the necessary Jenkins plugins: Git, Maven Integration, Pipeline, and Kubernetes Continuous Deploy.

     2. Created a new Jenkins pipeline and configured it with the Git repository URL for the Java application. 
        I have also added a Jenkinsfile to the Git repository to define the pipeline stages.

     3. Defined the pipeline stages, including checking out the source code from Git, building the Java application, 
     running unit tests and SonarQube analysis, packaging the application, deploying it to a test environment using Helm, 
     running user acceptance tests, and promoting it to a production environment using Argo CD.

     4. Configured the Jenkins pipeline stages to use the appropriate plugins for each stage.

     5. Set up Argo CD on the Kubernetes cluster, created a Git repository for Argo CD to track changes, 
     and created a Helm chart for the Java application that included Kubernetes manifests and Helm values.

     6.Configured the Jenkins pipeline to integrate with Argo CD by adding the Argo CD API token to Jenkins credentials 
     and updating the pipeline to include the Argo CD deployment stage.

     7. Ran the Jenkins pipeline, triggering the CI/CD process for the Java application, and 
     monitored the pipeline stages to ensure successful deployment

This end-to-end Jenkins pipeline will automate the entire CI/CD process for a Java application, from code checkout to production deployment, using popular tools like SonarQube, Argo CD, Helm, and Kubernetes.
