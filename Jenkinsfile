pipeline {
    agent any

    stages {

        stage('Cloner le code') {
            steps {
                echo 'Code déjà récupéré depuis GitHub'
            }
        }

        stage('Compiler') {
            steps {
                bat 'mvn clean compile'
            }
        }

        stage('Tests') {
            steps {
                bat 'mvn test'
            }
        }

        stage('Build') {
            steps {
                bat 'mvn package'
            }
        }
    }
}
