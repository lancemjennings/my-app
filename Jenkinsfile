pipeline {
    agent any
    stages {
        stage('---clean---') {
            steps {
                sh "mvn clean -f my-app"
            }
        }
        stage('---test---') {
            steps {
                sh "mvn test -f my-app"
            }
        }
        stage('--deploy---') {
            steps {
                sh "mvn package -f my-app"
            }
        }
    }
}
