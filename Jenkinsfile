node {
  checkout scm
  echo 'Pulling...' + env.BRANCH_NAME
  def dockerfile = 'Dockerfile-env.BRANCH_NAME'
  echo ${dockerfile}
#  stage('Do job stage') {
#    sh 'sudo docker run --rm -v ${WORKSPACE}:/var/app -w /var/app \
#    --volumes-from=ssh-agent -e SSH_AUTH_SOCK=/.ssh-agent/socket -v ${HOME}/.ssh/known_hosts:/etc/ssh/ssh_known_hosts \
#    pip install -requirements.txt'
#  }
}
