pipeline {
  agent any
  stages {
    stage('Preparacao') {
      steps {
        script {
          withEnv(["JAVA_HOME=${ tool 'jdk8-u144' }", "PATH+MAVEN=${tool 'maven'}/bin:${env.JAVA_HOME}/bin"]) {
            sh "mvn -version"
          }
        }
        
      }
    }
  }
}