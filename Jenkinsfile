pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Start building .....'
        input(message: 'Please hit return to continue', id: '1001')
        build 'make'
        waitForBuild '1001'
        echo 'build complete'
      }
    }

  }
}