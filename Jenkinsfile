pipeline {
    agent any
    stages {
        stage('Build container python') {
            steps {
                sh 'docker run -v $(pwd):$(pwd) python:3.5.1 python $(pwd)/helloweorld.py'
                sh 'docker rm -f mypython'
            }
        }
    }
}