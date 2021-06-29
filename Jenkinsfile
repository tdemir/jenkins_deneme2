pipeline {
  agent any
  stages {
    stage('docker-image-create') {
      steps {
        sh 'curl -fsSLO https://get.docker/builds/Linux/x86_64/docker-17.04.0-ce.tgz && tar xzvf docker-17.04.0-ce.tgz && mv docker/docker /usr/local/bin && rm -r docker docker-17.04.0-ce.tgz'
        sh 'docker version'
        sh 'docker build -t hello_wolrd .'
      }
    }

  }
}