pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Compiling Java file'
                bat 'javac ArmstrongNumbers.java'
            }
        }
        stage('Test') {
            steps {
                echo 'Running program'
                bat 'java ArmstrongNumbers'
            }
        }
    }
}
