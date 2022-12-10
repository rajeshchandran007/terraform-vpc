pipeline {
    agent any 
    stages {
        stage('Terraform Init') {
            steps {
                sh ""
                sh "terraform init --backend-config=env-dev/dev-backend.tfvars"
            }
        }

        stage('Terraform Plan') {
            steps {
                sh "terraform plan -var-file=env-dev/dev.tfvars"
            }
        }

    }
}