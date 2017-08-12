pipeline {
  agent any
  stages {
    stage('Preparacao') {
      steps {
        parallel(
          "Preparacao": {
            script {
              withEnv(["PATH+MAVEN=${tool 'maven'}/bin"]) {
                sh "mvn -version"
              }
            }
            
            
          },
          "Preparacao (mvn pipeline)": {
            withMaven(maven: 'maven') {
              sh 'mvn -version'
            }
            
            
          }
        )
      }
    }
  }
}