pipeline {
    agent any
    stages {
        stage('Build container python') {
            steps {
                sh 'docker run --name mypython  -v $(pwd):$(pwd) python:3.5.1 python $(pwd)/helloworld.py'
                sh 'docker rm -f mypython'
            }
        }
    }
}