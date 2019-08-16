pipeline {
    agent any
    tools {
        maven 'Maven'
        java 'Java'
    }
    stages { 
        stage('Example') {
            steps {
                sh 'mvn --version'
                sh 'java -version'
                echo 'Hello World'
                echo 'second time'
            }
        }
            stage('second example') {
            steps {
                echo 'this is saiteja'
            }
        }
    }
}

