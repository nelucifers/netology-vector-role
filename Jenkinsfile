pipeline {
    agent any
    stages {
        stage('Inatsll molecule') {
            steps {
                sh 'pip3 install "molecule==3.5.2"'
                sh 'pip3 install molecule_docker'
            }
        }
        stage('Get code') {
            steps {
                git branch: 'main', url: 'https://github.com/nelucifers/netology-vector-role.git'
            }
        }
        stage('Testing') {
            steps {
                sh 'molecule init scenario default --driver-name docker'
                sh 'molecule test'
            }
        }
    }
}
