pipeline{
        agent any
        stages{
                stage('Initial Setup'){
                        steps{
                                sh 'echo Starting...'
                        }
                }
                stage('Checking Docker'){
                        steps{
                                sh 'sudo docker ps'
								
                        }
                }
		stage('Build Docker'){
			steps{
				sh 'sudo docker build --tag=prueba .'
			}
		}
		stage('Deploy Container'){
			steps{
				sh 'sudo docker run -p 80:80 -- name Prueba1 --rm prueba'
			}
		}
	}
}
