pipeline {
    agent any

    stages {
        /*
        stage('build') {
            steps {
                sh 'docker --version'
                sh 'docker build -t minha_image .'
                sh 'docker run -p 88:80 -d minha_image'
            }
        }
        */
        stage('deploy') {
            steps {
                sh "chmod +x -R ${env.WORKSPACE}"
                sh "./script.sh"
            }
        }        
    }
}
