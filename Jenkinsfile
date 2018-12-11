
pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        step([$class: 'CopyArtifact', projectName: 'team-c/DevOptics-application-build'])
        archiveArtifacts artifacts: '*.sh', fingerprint: true
      }
    }
  }
}
