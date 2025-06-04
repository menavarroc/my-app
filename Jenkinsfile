pipeline {
    agent any
    stages {
        stage('---Clean---') {
            steps {
                sh "/opt/apache-maven-3.9.9/bin/mvn clean"
            }
        }
        stage('---Test---') {
            steps {
                sh "/opt/apache-maven-3.9.9/bin/mvn test"
            }
        }
        stage('---Deploy---') {
            steps {
                sh "/opt/apache-maven-3.9.9/bin/mvn package"
            }
        }
    }
}
