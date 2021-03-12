pipeline {
    agent any

    stages {
         stage('PrecheckInfra') {
            steps {
                echo 'Terraform apply'
                //sh 'sudo docker build -t laxman/webapp . '
            }
        }
         stage('Pre check environment') {
            steps {
                echo 'Ansible'
                //sh 'sudo docker build -t laxman/webapp . '
            }
        }
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'sudo docker build -t laxman/webapp . '
            }
        }
    
        stage('Deploy') {
            steps {
                echo 'kubectl apply -f '
            }
        }
    }
}
