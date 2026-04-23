pipeline {
    agent any

    triggers {
        pollSCM('* * * * *')
    }

    stages {

        stage('Clone Code') {
            steps {
                git 'https://github.com/SoyyalParveen/event-registration.git'
            }
        }

        stage('Build') {
            steps {
                bat 'build.bat'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment Successful'
            }
        }
    }
}