pipeline{
    agent any
    environment {
        PATH = "$PATH:/etc/apache-maven-3.8.6"
    }
    stages{
	stage('GetCode'){
            steps{
		git branch: 'main',
                url: 'https://github.com/ranjith120/mithuntechnoligieshelm.git'
            }
         }        
	stage('Build'){
            steps{
                sh 'mvn clean package'
            }
        }       
    }
}
