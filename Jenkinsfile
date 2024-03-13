pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build atomation'
        sh './cloud_user build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }      
    }
  }
}
