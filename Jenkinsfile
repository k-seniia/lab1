pipeline {
    agent any
    stages {
        stage('deploy') {
            steps {
                git url:'https://github.com/k-seniia/lab1.git', branch: "main"
                sh "aws configure set region us-east-1"
                sh "aws configure set aws_access_key_id ASIAVR6JY2OVAHQVAYNZ"  
                sh "aws configure set aws_secret_access_key 2no2N0pL+EobxvHpQj9kbSTQvNKVluIM6RoiVNg5"
                sh "aws s3 cp index.html s3://jenkins-bucket-i-0f46e30473a3f5d47"
            }
        }
    }
}
