pipeline {
    agent any
    stages {
        stage('Build container python') {
            steps {
                sh 'docker run --name mypython python:3.5.1 python ./helloworld.py'
                sh 'docker rm -f mypython'
            }
        }
    }
}