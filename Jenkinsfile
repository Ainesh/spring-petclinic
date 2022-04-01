pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh './mvnw clean package '
      }
    }

    stage('Run') {
      steps {
        sh '  java -jar target/*.jar &'
      }
    }

  }
}