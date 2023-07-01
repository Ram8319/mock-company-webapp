pipeline {
    agent any

    stages {
        stage('checkout') {
            steps {
                git 'https://github.com/Ram8319/devops-webapp.git'
            }
        }

        stage('gradle Build') {
          steps {
            withGradle {
              sh 'gradle build'
            }
          }
        }

        stage('gradle test') {
          steps {
            withGradle {
              sh 'gradle test'
            }
          }
        }
    }
}