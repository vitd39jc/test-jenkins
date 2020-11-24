pipeline {
  agent any

  tools {nodejs "node"}

  stages {
    stage('Nodejs stage') {
      steps {
        sh 'npm config ls'
        sh 'echo start pipeline'
        sh '''
           fdsfsd
           npm i
           npm i -g mocha
           npm run test
           exit
        '''
      }
    }
  }
}
