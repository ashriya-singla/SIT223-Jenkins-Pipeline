pipeline {
    agent any

    triggers {
        pollSCM('H/2 * * * *')
    }

    stages {

        stage('Build') {
            steps {
                echo 'Building application using Maven'
            }
        }

        stage('Unit and Integration Tests') {
            steps {
                echo 'Running Unit and Integration Tests using JUnit'
            }
        }

        stage('Code Analysis') {
            steps {
                echo 'Performing code quality analysis using SonarQube'
            }
        }

        stage('Security Scan') {
            steps {
                echo 'Scanning application using OWASP Dependency-Check'
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo 'Deploying application to AWS EC2 staging environment'
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo 'Running integration tests using Selenium'
            }
        }

        stage('Deploy to Production') {
            steps {
                echo 'Deploying application to AWS EC2 production environment'
            }
        }
    }
}
