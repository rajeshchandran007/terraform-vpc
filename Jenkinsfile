pipeline {
    agent any 
    stages {
        stage('Terraform Init') {
            steps {
                sh "terraform init --backend-config=env-dev/dev-backend.tfvars"
            }
        }

        stage('Terraform Plan') {
            steps {
                sh "terraform init --backend-config=env-dev/dev-backend.tfvars"
            }
        }

    }
}