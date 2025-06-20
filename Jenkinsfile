pipeline {
    agent any
    tools {
        maven 'maven 3.9.9'
    }
    stages {
        stage('---Clean---') {
            steps {
                sh "mvn clean"
            }
        }
        stage('---Test---') {
            steps {
                sh "mvn test"
            }
        }
        stage('---Deploy---') {
            steps {
                sh "mvn package"
            }
        }
    }
}
