 pipeline {
	agent any
	triggers {
		pollSCM ignorePostCommitHooks: true, scmpoll_spec: 'H/1 * * * *'
	}
	options {
	  buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '', daysToKeepStr: '7', numToKeepStr: '10')
	}
	stages {
		stage('Stage 1') {
			steps {
				script {
					echo 'echo Stage 111'
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
