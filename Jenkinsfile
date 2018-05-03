pipeline {
  agent any
  stages {
    stage('Check Functionality') {
      steps {
        ansiblePlaybook(playbook: 'cis-mikk.yml', become: true, becomeUser: 'mikk', colorized: true, tags: 'section5.2.2', credentialsId: '36d25621-d8c338e9-c819-4fc8-898a-a5f5313a4d4e', vaultCredentialsId: '6b976b74-3e55-436d-afd2-9b33d2d5ead7')
      }
    }
  }
}