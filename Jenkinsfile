pipeline {
  agent any

  tools {nodejs "node"}

  stages {
    stage('Nodejs stage') {
      steps {
        sh 'npm config ls'
        sh 'echo start pipeline'
        sh '''
           npm i
           npm i -g mocha
           npm run test
           exit
        '''
      }
    }
  }
}
