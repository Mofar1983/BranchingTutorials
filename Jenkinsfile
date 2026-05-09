pipeline {
    agent any 

    stages {
        stage('Checkout') {
            steps {
                // This pulls your code from GitHub
                checkout scm
            }
        }
        stage('Verify File') {
            steps {
                echo 'Checking if AdminService.txt exists...'
                // Using Windows batch command (bat)
                bat 'type AdminService.txt'
            }
        }
        stage('Build') {
            steps {
                echo 'Simulating Build Process...'
                // You would put your javac or npm build commands here
            }
        }
    }
}