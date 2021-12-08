pipeline {

    stages {
        stage('Build') {
            steps {
                // Get some code from a GitHub repository
                git "https://github.com/Charaniy/ecs-fargate.git"
                sh "terraform init"
                sh "terraform plan"
                sh "terraform apply=target=main.tf --auto-approve=true"

            }
           
        }
    }
}
