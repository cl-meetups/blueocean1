pipeline {
  agent any
  stages {
    stage('Preparacao') {
      steps {
        script {
          withEnv(["PATH+MAVEN=${tool 'maven'}/bin"]) {
            sh "mvn -version"
          }
        }
        
      }
    }
  }
}