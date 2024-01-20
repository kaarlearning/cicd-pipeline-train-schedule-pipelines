pipeline {
  agent any
  stages {
    stage ('Build'){
      steps {
        echo 'Running Automated build'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
