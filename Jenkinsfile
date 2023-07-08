
pipeline {
  agent any
    stages {
        stage('Pull') {
             steps{
                script{
                    checkout([$class: 'GitSCM', branches: [[name: '*/main']],
                        userRemoteConfigs: [[
                            credentialsId: 'c82b8134-5b85-4432-a000-887da1bb9464',
                            url: 'https://github.com/haifgh/Myapp.git']]])
                }
            }
        }
    }
}
