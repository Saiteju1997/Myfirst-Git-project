pipeline {
    agent any
    tools {
        maven 'Maven'
    }
    stages { 
        stage('Example') {
            steps {
                sh 'mvn --version'
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

