pipeline {
  agent any
  stages {
    stage('docker-image-create') {
      steps {
        sh 'docker build -t hello_wolrd .'
      }
    }

  }
}
