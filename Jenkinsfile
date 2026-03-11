pipeline {
    agent any

    stages {

        stage('Terraform Init') {
            steps {
                sh '/opt/homebrew/bin/terraform init'
            }
        }

        stage('Terraform Validate') {
            steps {
                sh '/opt/homebrew/bin/terraform validate'
            }
        }

        stage('Terraform Plan') {
            steps {
                sh '/opt/homebrew/bin/terraform plan'
            }
        }

        stage('Terraform Apply') {
            steps {
                sh '/opt/homebrew/bin/terraform apply -auto-approve'
            }
        }

    }
}
