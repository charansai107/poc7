pipeline {
    agent any

    stages {

        stage('Clone Code') {
            
 steps {
        git branch: 'main',
            url: 'https://github.com/charansai107/poc7.git'
    }

        }

        stage('Deploy Using Ansible') {
            steps {
                sh 'ansible-playbook deployment.yml'
            }
        }
    }
}
