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
				sh 'pwd'
				sh cp -r d4a/code/Dockerfile /var/jenkins/home/workspace/Pipeline EDSI
                        }
                }
	}
}
