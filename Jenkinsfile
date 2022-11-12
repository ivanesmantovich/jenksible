pipeline {
	agent any
	
	stages {
		stage("changes-download") {
			if (env.GIT_COMMIT != env.GIT_PREVIOUS_SUCCESSFUL_COMMIT) {
				echo "THERE IS A CHANGEEEEEEEEEEEEEEEEEEEEEEEEEEEEEE"
			}
		}
		stage("changes-zip") {
		}
		stage("invoke-next-pipeline") {
		}
	}
}
