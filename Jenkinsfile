pipeline {
    agent any 
    stages {
        stage('Git Clone') {
            steps {
                sh "mvn clean -f Springboot-App"
            }
        }
        stage('Demo') {
            steps {
                sh "mvn test -f Springboot-App"
            }
        }
        stage('Deploy') { 
            steps {
                sh "mvn package -f Springboot-App"
            }
        }
    }
}
