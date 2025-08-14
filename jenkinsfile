pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                // Pull source code from Git
                git branch: 'main', url: 'https://github.com/Savita-Nalawade/simple-java-application'
            }
        }

        stage('Build') {
            steps {
                script {
                    sh 'javac Hello.java'
                }
            }
        }

        stage('Run') {
            steps {
                script {
                    sh 'java Hello'
                }
            }
        }
    }
}:
:wq!
[A[C[C[A[C