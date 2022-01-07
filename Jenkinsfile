pipeline {
  agent any
  stages {
    stage('clone') {
      steps {
        sh 'sudo git clone https://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@github.com/Hemajo/docker-terraform.git'
      }
    }

    stage('execution') {
      steps {
        sh '''sh terraform init
sh terraform plan
sh terraform apply auto --approve'''
      }
    }

  }
}