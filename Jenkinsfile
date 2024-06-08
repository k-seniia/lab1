pipeline {
  agent any
  stages {
    stage('Deploy to S3') {
      steps {
        git url:'https://github.com/k-seniia/lab1.git', branch: "main"
        sh "aws s3 cp index.html s3://jenkins-bucket-i-0f46e30473a3f5d47"
      }
    }
  }
}
