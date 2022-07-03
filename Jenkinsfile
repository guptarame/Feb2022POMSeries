pipeline {
    agent any
 tools {
        maven "MAVEN_HOME"
    }
    stages {
        stage('Build') {
            steps {
                git credentialsId: '5b9319da-8c4f-4392-8560-98d63bbc8bfc', url: 'https://github.com/guptarame/Feb2022POMSeries.git'
            }
        }
        stage('Compile') {
            steps {
                sh 'mvn compile'
            }
        }
        stage('Unit Test') {
            steps {
                echo 'mvn test'
            }
        }
        stage('Integration Test Hello') {
            steps {
                echo 'Integration Test World'
            }
        }
        stage('Result') {
            steps {
                junit '**/*.xml'
            }
        }

         stage('package') {
            steps {
                sh 'mvn package'
            }
        }


         stage('Deploy War File ') {
            steps {
                echo 'Deploy war file World'
            }
        }

    }
}
