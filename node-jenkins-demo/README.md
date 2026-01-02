# Node.js Jenkins Pipeline Demo 🚀

This project demonstrates how to build and run a Node.js application using Jenkins Pipeline with Docker.

---

## Project Structure

```
node-jenkins-demo/
├── app.js
├── package.json
├── Jenkinsfile
└── README.md
```



---

## Prerequisites

- Jenkins installed
- Docker installed and configured
- Jenkins Docker plugin enabled
- GitHub repository access

---

## Jenkins Job Configuration

- **Job Type:** Pipeline  
- **Definition:** Pipeline script from SCM  
- **SCM:** Git  
- **Repository URL:**
- **Branch Specifier:**
*/main
- **Script Path:**
node-jenkins-demo/Jenkinsfile
---
## What Happens After Build Now

- Jenkins creates a workspace
- GitHub repository is cloned
- Jenkinsfile is read
- Docker container is started
- Pipeline stages run inside container
- Container is stopped and removed
---

## Build result is shown
- v16.20.2
- Hello from Node.js app running in Jenkins 🚀
- Finished: SUCCESS

