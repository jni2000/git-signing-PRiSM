pipeline {
  agent any
  stages {
    stage('Build') {
      agent any
      steps {
        echo 'Start building .....'
        input(message: 'Please hit return to continue', id: '1001')
        build 'cd workspace/git-signing-PRiSM'
        waitForBuild '1001'
        echo 'build complete'
      }
    }

  }
}