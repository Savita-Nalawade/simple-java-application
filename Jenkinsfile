pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Pull source code from Git
                git branch: 'master', url: 'https://github.com/Savita-Nalawade/simple-java-application'
            }
        }

        stage('Build') {
            steps {
                // Compile and package Java project
                bat 'javac HelloWorld.java'
            }
        }

        stage('Run') {
            steps {
                // Run the generated JAR file
                bat 'java HelloWorld'
            }
        }
    }
}
