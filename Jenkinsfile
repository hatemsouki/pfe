pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
              
                sh  
                archiveArtifacts artifacts: '**/apptest/*.php', fingerprint: true 
           
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
