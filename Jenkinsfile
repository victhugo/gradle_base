pipeline {
  agent any
  stages {
    stage('Unit & Integration') {
      agent any
      steps {
        echo 'Make gradlew executable'
        sh 'chmod +x ./gradlew'
        echo 'Running ...'
        sh './gradlew clean test --no-daemon'
      }
    }

    stage('Build') {
      steps {
        echo 'Build the projecct'
        sh 'chmod +x ./gradlew'
        sh './gradlew build'
      }
    }

  }
}