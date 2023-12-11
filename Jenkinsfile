pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                // Compile the Java application
                bat "javac -cp . main.java"
            }
        }

        stage('Run') {
            steps {
                // Run the Java application
                bat 'java -cp . main'
            }
        }
    }
}
