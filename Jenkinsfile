pipeline {
  agent {
    node {
      label 'vm1'
    }
  }

  stages {
    stage('test docker commands') {
      steps {
        sh "echo '------------Examine ops stack------------'"
        sh "docker node ls"
        sh "docker stack deploy -c stack.yml web"
        }
    }
  }
}