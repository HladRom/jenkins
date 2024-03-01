# TASK :star: :star: :star:
## Jenkins
1.  Run Jenkins in the local environment, configure it.
2.  Download the GIT repository.
3.  The process of building the project (Preparation of npm install).
4.  Building a docker container.
5.  Uploading the container to DockerHub.
6.  Starting the container.

### Code:

### jenkins
**its for jenkins task, bild progekt (VPD).**
```python
`stages {`
        `stage('cloning our GIT') {`
            `steps {`
                `git url: "https://github.com/HladRom/-vue-paper-dashboard"`
            `}`
        `}`
        `stage('Pre-Build preparations') {`
            `steps {`
                `sh "npm install"`
    `}`
`}`
        `stage('Build app & docker image') {`
            `steps {`
                `sh "npm run build"`
    `}`
`}`
      
    `}`
`}`
```
![myjenki](https://cdn.iconscout.com/icon/free/png-256/free-jenkins-282182.png?f=webp)
