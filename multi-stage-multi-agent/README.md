# Jenkins Multi-Agent Docker Pipeline

This Jenkins Declarative Pipeline demonstrates how different stages can run
inside **different Docker containers** for back-end and front-end tasks.

## Pipeline Overview
- Uses `agent none` to disable a global agent
- Runs each stage in its **own Docker environment**
- Back-end uses **Maven + Java**
- Front-end uses **Node.js**

## Syntax Explanation (Brief)

- `pipeline {}` → Defines the Jenkins pipeline
- `agent none` → No global agent; agents are defined per stage
- `stages {}` → Contains multiple stages
- `stage('Back-end')` → Back-end build stage
- `docker { image 'maven:3.8.1-adoptopenjdk-11' }` → Docker image for Maven & Java
- `sh 'mvn --version'` → Prints Maven version
- `stage('Front-end')` → Front-end build stage
- `docker { image 'node:16-alpine' }` → Docker image for Node.js
- `sh 'node --version'` → Prints Node.js version
