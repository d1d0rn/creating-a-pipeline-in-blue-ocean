pipeline {
  agent {
    docker {
      image 'node:6-alpine'
      args '-p 3000:3000'
    }
    
  }
  stages {
    stage('buildd') {
      steps {
        sh 'npm install'
      }
    }
    stage('ttest') {
      steps {
        input(message: 'ok?', id: 'okkk', ok: 'o_k')
      }
    }
  }
}