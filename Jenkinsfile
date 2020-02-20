pipeline {
  agent any
  stages {
    stage('Build') {
      agent any
      steps {
        echo 'Running ...'
        withGradle() {
          echo 'Make gradlew executable'
          sh 'chmod +x ./gradlew'
          sh './gradlew clean test --no-daemon'
        }

      }
    }

  }
}