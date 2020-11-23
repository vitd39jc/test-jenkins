pipeline {
  agent any
 
  tools {nodejs "node"}
 
  stages {
    stage('Example') {
      steps {
        sh 'npm config ls'
        sh 'echo start pipeline'
        sh '''
           echo "Multiline shell steps works too"
           npm i npm@latest -g
           npm i -g pm2
           pm2 start ecosystem.config.js
           pm2 restart all
        '''
      }
    }
  }
}
