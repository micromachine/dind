pipeline {
  agent {
    docker {
      image 'python:3.7.3'
      args '--volumes-from=ssh-agent -e SSH_AUTH_SOCK=/.ssh-agent/socket -v ${HOME}/.ssh/known_hosts:/etc/ssh/ssh_known_hosts'
    }
  }
  stages {
    stage('Do job stage') {
      steps {
        sh "pip install -requirements.txt"
      }
    }
  }
}
