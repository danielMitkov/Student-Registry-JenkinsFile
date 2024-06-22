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
        stage("Integration tests"){
            steps{
                bat 'npm run test'
            }
        }
    }
}