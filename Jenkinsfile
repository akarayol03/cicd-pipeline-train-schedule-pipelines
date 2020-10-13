pipeline{
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-daemon'
        archiveArthifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
