
pipeline {
    agent any 
    stages {
        stage('Build') {
            steps {
                bat 'make'
                archiveArtifacts artifacts:'**/build1/*.jar',fingerprint: true
            }
        }
        stage('Test'){
            steps{
            echo 'Testing'
            }
        }
        stage('Deploy'){
            steps{
            echo 'Deploying'
            }
        } 
    }
    
}
