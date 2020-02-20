pipeline {
  agent any
  stages {
    stage('Build') {
      agent any
      steps {
        echo 'Make gradlew executable'
        sh 'chmod +x ./gradlew'
        echo 'Running ...'
        sh './gradlew clean test --no-daemon'
      }
    }

  }
}