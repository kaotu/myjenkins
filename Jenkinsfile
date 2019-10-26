pipeline {
    agent any
    stages {
        stage('Build container python') {
            steps {
                sh 'docker run --name mypython  -v $(pwd):/var/ python:3.5.1 python /var/helloworld.py'
                sh 'docker rm -f mypython'
            }
        }
    }
}