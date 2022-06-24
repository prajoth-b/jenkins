pipeline {
    agent any 
    stages {
        stage('Git Clone') {
            steps 
                git branch: 'fs', url: 'https://github.com/prajoth-b/jenkins.git'
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
