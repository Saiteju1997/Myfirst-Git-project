pipeline {
    agent any
    tools {
        maven 'Maven'
        jdk 'Java'
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
        stage('build') {
            steps {
                sh 'mvn install'
                sh 'deploy'
            }
        }
    }
}

