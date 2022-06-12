pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'building'
        sh 'mvn compile'
      }
    }

    stage('test') {
      steps {
        sh 'mvn test'
      }
    }

    stage('package') {
      steps {
        sh 'mvn package'
      }
    }

  }
}