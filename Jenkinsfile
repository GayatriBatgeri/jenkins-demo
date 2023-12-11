pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout your source code from version control
                checkout scm
            }
        }

        stage('Build') {
            steps {
                // Compile the Java application
                sh 'javac -cp . src/Main.java'
            }
        }

        stage('Run') {
            steps {
                // Run the Java application
                sh 'java -cp . src/Main'
            }
        }
    }
}
