pipeline {
    agent any

    stages {

        stage('Clone Code') {
            steps {
                git 'https://github.com/<username>/<repo>.git'
            }
        }

        stage('Deploy Using Ansible') {
            steps {
                sh 'ansible-playbook deployment.yml'
            }
        }
    }
}
