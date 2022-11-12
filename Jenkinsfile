pipeline {
	agent any
	
	stages {
		stage("changes-download") {
			steps {
				git credentialsId: 'jenksible_id', url: 'https://github.com/ivanesmantovich/jenksible'
			}
		}
	}
}
