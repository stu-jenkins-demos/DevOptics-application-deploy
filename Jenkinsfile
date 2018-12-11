
pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        step([$class: 'CopyArtifact', projectName: 'team-c/DevOptics-application-build/master'])
        archiveArtifacts artifacts: '*.sh', fingerprint: true
      }
    }
  }
}
