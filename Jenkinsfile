pipeline {
  agent any
  stages {
    stage('Check Functionality') {
      steps {
        ansiblePlaybook(playbook: 'cis-mikk.yml', becomeUser: 'mikk', colorized: true, tags: 'section5.2.2', credentialsId: '36d25621-624c-4d97-a1e4-aac84f6fe071', vaultCredentialsId: '6b976b74-3e55-436d-afd2-9b33d2d5ead7', extras: '-C')
      }
    }
  }
}