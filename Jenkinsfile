pipeline {
  agent {
    node {
      label 'ansibletest-1'
    }

  }
  stages {
    stage('Check Functionality') {
      steps {
        ansiblePlaybook(playbook: 'cis-mikk.yml', become: true, becomeUser: 'mikk', colorized: true, tags: 'section5.2.2')
        ansibleTower()
      }
    }
  }
}