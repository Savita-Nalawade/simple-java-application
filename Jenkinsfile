pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'master',
                    url: 'https://github.com/Savita-Nalawade/simple-java-application.git',
                    credentialsId: 'Github-Creds'
            }
        }

        stage('Build') {
            steps {
                // Compile and package Java project
                bat 'mvn clean package'
            }
        }

        stage('Run') {
            steps {
                // Run the generated JAR file
                bat 'java -jar target/*.jar'
            }
        }
    }
}
