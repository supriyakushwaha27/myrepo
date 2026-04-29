pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Compiling Java file'
                sh 'javac ArmstrongNumbers.java'
            }
        }
        stage('Test') {
            steps {
                echo 'Running program'
                sh 'java ArmstrongNumbers'
            }
        }
    }
}
