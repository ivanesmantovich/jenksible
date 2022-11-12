pipeline {
	agent any
	
	stages {

		if (env.GIT_COMMIT != env.GIT_PREVIOUS_SUCCESSFUL_COMMIT) {
			stage("changes-download") {
				echo "there is a change"
				sh 'git clone'
					
			}

			stage("changes-zip") {
				
			}

			stage("invoke-next-pipeline") {
				
			}
		}
	}
}
