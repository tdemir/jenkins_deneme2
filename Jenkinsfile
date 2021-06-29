pipeline {
  agent any
  stages {
    stage ('Docker') {
      steps {
        sh 'docker version'
      }
    }
    stage('docker-image-create') {
      steps {
        sh 'docker build -t hello_wolrd .'
      }
    }

  }
}
