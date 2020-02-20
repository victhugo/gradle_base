pipeline {
  agent any
  stages {
    stage('Build') {
      agent any
      steps {
        echo 'Running ...'
        withGradle() {
          sh './gradlew clean test --no-daemon'
        }

      }
    }

  }
}