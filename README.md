# TASK :star: :star:  :star:


## Introduction
In this project, we will explore the process of using Jenkins to automate various steps in software development and deployment. We'll cover steps from running Jenkins in the local environment to uploading a container to DockerHub and starting it. This process greatly simplifies and accelerates software development and deployment.

## Project Steps
- Run Jenkins in the local environment and configure it: Install and run Jenkins on your local machine. Configure Jenkins according to your project's needs.

- Download the GIT repository: Using Jenkins, download your project's code from the GIT repository. This can be done using an appropriate plugin or Git command.

- Build the project (Preparation of npm install): Build your project. This step may include setting up the environment to execute the npm install command or any other preparatory work.

- Build Docker container: Using Jenkins, build a Docker container for your project. You will need a Dockerfile to define the container's configuration.

- Upload the container to DockerHub: After building the container, upload it to DockerHub so that other users can easily access it.

- Start the container: Finally, using Jenkins, start the uploaded container on the desired server or host.

## Conclusion
Using Jenkins to automate the software development and deployment process greatly simplifies and accelerates workflows. From running Jenkins and downloading code from GIT to building a Docker container, uploading it to DockerHub, and starting it - this process provides an efficient and automated workflow.
### Code:

### jenkins
**its for jenkins task, bild progekt (VPD).**
```python
stages {
        stage('cloning our GIT') {
            steps {
                git url: "https://github.com/HladRom/-vue-paper-dashboard"
            }
        }
        stage('Pre-Build preparations') {
            steps {
                sh "npm install"
    }
}
        `stage('Build app & docker image') {
            steps {
                sh "npm run build"
    }
}
      
    }
}
```
![myjenki](https://cdn.iconscout.com/icon/free/png-256/free-jenkins-282182.png?f=webp)
