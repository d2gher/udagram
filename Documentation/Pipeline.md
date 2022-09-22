# CircleCI pipeline

This project uses CircleCI for the CD part of the CI/CD process

## The process 

It starts whenever any change happens to the main branch in our github repo 

### Orbs

- Installs node.js
- Installs AWS-CLI
- installs EB

### Workflow

#### Build

- Installs the dependencies the fornt and backend need
- Testing
- Building the files that we will deploy

#### Hold

Makes the pipeline wait for aprovel before deploying the app

#### Deploy 

- Sets the environment variables
- Deploys the backend
- Deploys the frontend
