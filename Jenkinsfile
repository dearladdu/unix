pipeline {
    agent none
    stages {
        stage('update') {
            steps {
               sh 'sudo apt update'
            }
        }
        stage('Install Dependency') {
            steps {
               sh 'sudo apt install software-properties-common'
            }
        }   
        stage('Add repo') {
            steps {
               sh 'sudo add-apt-repository ppa:deadsnakes/ppa -y'
            }
        }
        stage('Install Python') {
            steps {
               sh 'sudo apt install python3.7'
            }
        }
         stage('Python version') {
            steps {
               sh 'python3.7 --version'
            }
        }
    }
}
