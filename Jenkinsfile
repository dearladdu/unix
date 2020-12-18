pipeline {
    agent any
    stages {
        stage('update') {
            steps {
               sh 'apt update'
            }
        }
        stage('Install Dependency') {
            steps {
               sh 'apt install software-properties-common'
            }
        }   
        stage('Add repo') {
            steps {
               sh 'add-apt-repository ppa:deadsnakes/ppa -y'
            }
        }
        stage('Install Python') {
            steps {
               sh 'apt install python3.7'
            }
        }
         stage('Python version') {
            steps {
               sh 'python3.7 --version'
            }
        }
    }
}
