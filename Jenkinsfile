pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Running ...'
        sh './gradlew clean test --no-daemon'
      }
    }

  }
}