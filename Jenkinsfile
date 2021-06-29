pipeline {
  agent any
  stages {
    stage ('docker_install') {
      steps {
        sh 'RUN curl -fsSLO https://get.docker/builds/Linux/x86_64/docker-17.04.0-ce.tgz && tar xzvf docker-17.04.0-ce.tgz && mv docker/docker /usr/local/bin && rm -r docker docker-17.04.0-ce.tgz'
      }
    }
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
