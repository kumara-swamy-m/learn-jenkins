# Jenkins Docker Pipeline code

This project demonstrates a simple **Jenkins Declarative Pipeline**
that runs inside a **Docker container** using Node.js.

## Jenkinsfile Explanation

### Pipeline Structure
- `pipeline {}` defines the Jenkins pipeline
- `agent { docker { ... } }` tells Jenkins to run the job in a Docker container
- `node:16-alpine` is a lightweight Node.js image
- `stages {}` contains pipeline stages
- `stage('Test')` defines a testing stage
- `sh 'node --version'` executes a shell command inside the container
