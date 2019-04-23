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
		stage('Build Container'){
			steps{
				sh 'sudo docker build --tag=Prueba .
			}
		}
		stage('Deploy Container'){
			steps{
				sh 'sudo docker run -p 80:80 --name phpedsi --rm Prueba
			}
		}
        }
}
