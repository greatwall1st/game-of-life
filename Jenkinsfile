 pipeline {
	agent any
	triggers {
		pollSCM ignorePostCommitHooks: true, scmpoll_spec: 'H/2 * * * *'
	}
	options {
		buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '', daysToKeepStr: '7', numToKeepStr: '10')
	}
	stages {
		stage('Stage 1') {
			steps {
				script {
					echo "Running stage 1 from ${env.NODE_NAME} on on ${env.JENKINS_URL}"
				}
			}
		}
		stage('Stage 2') {
			steps {
				script {
					echo 'echo Stage 222'
				}
			}
		}
	}
}
