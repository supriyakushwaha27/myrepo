pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Fetching code from GitHub'
                git 'https://github.com/supriyakushwaha27/myrepo.git'
            }
        }

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

    post {
        success {
            echo 'Build Successful!'
        }
        failure {
            echo 'Build Failed!'
        }
    }
}