pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running Build automation'
        sh './gradlew build --no-daemon'
        archieveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
