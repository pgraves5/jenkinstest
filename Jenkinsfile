library 'SharedLibs'

pipeline {
  agent {
    docker {
      image 'maven:alpine'
    }
    
  }
  stages {
    stage('mvn-version') {
      steps {
        sh 'mvn -v'
      }
      stage('Shared Lib') {
         steps {
             helloWorld("Jenkins")
         }
      }
    }
  }
}
