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
