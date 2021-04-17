 pipeline {
  agent any
  triggers {
    pollSCM ignorePostCommitHooks: true, scmpoll_spec: 'H/5 * * * *'
  }
  stages {
  stage('Stage 1') {
      steps {
        script {
          echo 'echo Stage 11'
        }
      }
    }
  stage('Stage 2') {
      steps {
        script {
          echo 'echo Stage 22'
        }
      }
    }
  }
}
