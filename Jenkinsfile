pipeline {
    agent any
    stages {
        stage('Build container python') {
            steps {
                sh 'docker run --name mypython python:3.5.1 print("Helloworld")'
                sh 'docker rm -f mypython'
            }
        }
    }
}