pipeline {
    agent any
    tools {
        maven 'Maven'
        jdk 'Java'
    }
    stages {
        stage('buildStage') {
            steps {
                echo "Building a maven project........!"
                sh 'mvn compile'
            }
        }
        stage('testingCode') {
            steps {
                echo "Testing........!"
                sh 'mvn test'
            }
        }
        stage('Clean up the Environment') {
            steps {
                echo "Cleaning up........!"
                cleanWs()
            }
        }
        
    }
}
