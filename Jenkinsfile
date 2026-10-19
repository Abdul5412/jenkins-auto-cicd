pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Jenkins is checking out the project!'
            }
        }

        stage('Test HTML') {
            steps {
                sh 'test -f index.html'
                sh "grep -q 'CRC Jenkins CI/CD Project' index.html"
                echo 'HTML test passed!'
            }
        }

        stage('Build') {
            steps {
                echo 'Build completed successfully!'
            }
        }
    }
}
