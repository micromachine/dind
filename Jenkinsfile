node {
  stage('Do job stage') {
    sh 'docker run --rm -v ${WORKSPACE}:/var/app -w /var/app \
    --volumes-from=ssh-agent -e SSH_AUTH_SOCK=/.ssh-agent/socket -v ${HOME}/.ssh/known_hosts:/etc/ssh/ssh_known_hosts \
    pip install -requirements.txt'
  }
}
