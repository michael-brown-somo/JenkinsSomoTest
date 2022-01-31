pipeline {
  agent any
  stages {
    stage('Login') {
      steps {
        bat 'sfdx auth:jwt:grant --instanceurl ${SF_INSTANCE_URL} --clientid ${SF_CONSUMER_KEY} --username ${SF_USERNAME} --jwtkeyfile ${server_key_file} --setdefaultdevhubusername --setalias main'
        powershell(script: 'sfdx force:org:display -u ${SF_USERNAME}', returnStatus: true)
      }
    }

  }
}