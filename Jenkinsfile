pipeline {
  agent any
  stages {
    stage('check') {
      steps {
        sh 'env'
        addBadge(icon: 'ok', text: 'ok')
      }
    }
    stage('build') {
      steps {
        sh 'git status'
        dir(path: 'jenkins') {
          echo 'In jenkins folder'
          sh 'ls -la'
        }

      }
    }
  }
}