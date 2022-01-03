pipeline {
  agent any
  stages {
    stage('error') {
      parallel {
        stage('error') {
          steps {
            sh '''./mvnw package
'''
          }
        }

        stage('check pmd') {
          steps {
            sh './mvnw pmd:check'
          }
        }

      }
    }

  }
}