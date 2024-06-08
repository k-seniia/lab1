pipeline {
    agent any
    stages {
        stage('deploy') {
            steps {
                git url:'https://github.com/k-seniia/lab1.git', branch: "main"
                //sh "aws configure set region us-east-1"
                //sh "aws configure set aws_access_key_id ASIAVR6JY2OVAHQVAYNZ"  
                //sh "aws configure set aws_secret_access_key 2no2N0pL+EobxvHpQj9kbSTQvNKVluIM6RoiVNg5"
                //sh "aws configure set aws_session_token IQoJb3JpZ2luX2VjEIL//////////wEaCXVzLXdlc3QtMiJIMEYCIQCLO/wNbDm3cY4kwDlCXszVHehUZVe3ZKwABqZl1D45VAIhAOjngez6UVggBwNHlKkOFluhjcu1/ciBxibCoQBuNs/7KqcCCBoQABoMMzgyMTM4MzczMDM0Igxwu4d1icitwZ2RUcwqhAINTsJZ5NLMvdT+ddxlVilGwfks7jrQhwX6OmBiI1P2YnRYRDryyfYHiQ6EcosYcC/UCDxtz/9Jf+miDmimYWHxGDDQVSk3tv+4e/FFaMQgXGtn086L6zL8lkhptYx6BIVBa2mIaFGunTlqjcoCeUNW3cadBxEcWKqKgBhGTPaC4hE8Gr9hjvTM6vZNyWELXhOZpyfM6xJY2F32zfdGFPWyPZ9pyNjUgTevqe5IN/4eU0qBo126dlG+0j8H/lVwrJpkeORKiqWltmMyGEdZDRIXjqGROp1i12Sdm9y/kfj4qwlUFNw/rQG1zAo3vvnSED3D7Jiq1NzJSxPlty+WEKf5+GD4KzCupZKzBjqcAeBxW/AJs/BtZqPDBp0WaYV3oY9WewC0UiAC8N4c188ZazGHiBMbOCkui8YKuHa+YQ4AX5pah2XODeLC4Rh2XH77tnmtS0/WupJgQ39gtoX0eW/lslFOTtldGhveMlwdYgogRUYcQEuHDFOSFkjH0wRurD5TWyDEJw2mBTUH71KHPPrUUGFx3dzU6ExgIVplzLrOAQRFW+lF2PSIIA=="
                sh "aws s3 cp index.html s3://jenkins-bucket-i-hetman"
            }
        }
    }
}
