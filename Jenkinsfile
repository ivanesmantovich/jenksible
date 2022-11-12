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
				sh "cd /var/lib/jenkins/workspace/jenksible_master && zip -r /abcde/distr/abc-v.${env.BUILD_NUMBER}.zip ."
			}	
		}
		stage("launch-ansible") {
			steps {
				ansiblePlaybook become: true, extras: '--extra-vars "version=${env.BUILD_NUMBER}"', playbook: 'jenksible.yml'
			}
		}
	}
}
