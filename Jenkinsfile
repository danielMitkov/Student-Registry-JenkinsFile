pipeline{
    agent any
    stages{
        stage("Install Dependancies"){
            steps{
                bat 'npm install'
            }
        }
        stage("Audit Vulnerabilities"){
            steps{
                bat 'npm audit fix --force'
            }
        }
    }
}