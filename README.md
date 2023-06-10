TASK
Task 3 Ansible
1.  Write a playbook that would install Jenkins and create a job in it: Pipeline.
2.  Since the job uses Docker, use Ansible to copy the required local files (Dockerfile) to the remote server.

# jenkins
its for jenkins task, bild progekt (VPD).
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
        stage('Build app & docker image') {
            steps {
                sh "npm run build"
    }
}
      
    }
}
