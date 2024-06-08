pipeline {
    agent any
    pipeline {
        agent any
        stages {
            stage('deploy') {
                steps {
                  git url:'https://github.com/k-seniia/lab1.git', branch: "main"
                  sh "aws configure set region us-east-1" 
                  shared_credentials_files = ["../s3_website/credentials"]
                  sh "aws s3 cp index.html s3://jenkins-bucket-i-0f46e30473a3f5d47"
                }
            }
        }
    }
}
