pipeline {
  agent none
  stages {
    stage('pull') {
      steps {
        sh '''pwd
ls -al'''
        ansiblePlaybook(playbook: 'test', becomeUser: 'root', colorized: true, become: true)
      }
    }
  }
}