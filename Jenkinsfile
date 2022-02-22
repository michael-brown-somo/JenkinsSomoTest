pipeline {
  agent any
  stages {
    stage('Login') {
      steps {
        sh '''#!/bin/bash
                sfdx auth:jwt:grant --instanceurl https://mindful-panda-s6hnbj-dev-ed.my.salesforce.com --clientid 3MVG9riCAn8HHkYXmQO2qmGWgar7bsQHV.2PradWPB2pVTH77tLDP2datbR3zmnjGi5AnXfcXN13eXlUb.bGt --username lgranadoscuello@mindful-panda-s6hnbj.com --jwtkeyfile **** --setdefaultdevhubusername --setalias main
                sfdx force:org:display -u ${SF_USERNAME}
           '''
      }
    }

  }
}