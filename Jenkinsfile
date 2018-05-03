pipeline {
  agent any
  stages {
    stage('Check Functionality') {
      steps {
        ansiblePlaybook(playbook: 'cis-mikk.yml', become: true, becomeUser: 'mikk', colorized: true, tags: 'section5.2.2', credentialsId: 'a15771a4-4c03-40b8-996b-913dec32dc97', vaultCredentialsId: '6b976b74-3e55-436d-afd2-9b33d2d5ead7')
      }
    }
  }
}