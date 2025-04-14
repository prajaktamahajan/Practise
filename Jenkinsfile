pipeline {
    agent any
    tools {
        maven 'maven_3.9.9'  // Match the name you gave in Jenkins
    }
    stages {
        stage('Maven Clean Build') {
            steps {
                echo 'Building...'
                 bat 'mvn -f demo\\pom.xml clean install'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                bat 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
            }
        }
    }
}
