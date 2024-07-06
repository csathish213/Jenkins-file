pipeline {
    agent any
    
    stages {
        stage('checkout') {
            steps {
                git 'https://github.com/csathish213/java-hello-world-with-maven-jenkin.git'
            }
        }
        stage('build') {
            steps {
                sh 'mvn compile'
            }
        }
        stage('test') {
            steps {
                sh 'mvn test'
            }
        }
        stage('artifact') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}
