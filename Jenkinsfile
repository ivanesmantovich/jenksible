pipeline {
	agent any
	
	stages {
		stage("download") {
			steps {
				git credentialsId: 'jenksible_id', url: 'https://github.com/ivanesmantovich/jenksible'
			}
		}

		stage("move-and-zip") {
			steps {
				sh "cd /var/lib/jenkins/workspace && zip /abcde/distr/abc-v.${env.BUILD_NUMBER}.zip jenksible_master"
			}	
		}
	}
}
