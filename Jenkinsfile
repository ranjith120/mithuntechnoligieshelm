pipeline{
    agent any
    environment {
        PATH = "$PATH:/etc/apache-maven-3.8.6"
    }
    stages{
	stage('GetCode'){
            steps{
		git branch: 'main',
                url: ''
            }
         }        
	stage('Build'){
            steps{
                sh 'mvn clean package'
            }
        }       
    }
}
