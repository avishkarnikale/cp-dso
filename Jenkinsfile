pipeline {
  agent any 
  stages {
    stage('Check secrets'){
      steps {build 'Git-Secrets'}
    }
    stage('Check dependencies'){
      steps {build 'OWASP-DEP-CHECK'}
    }
    stage('Check XSS with ZAP'){
      steps {build 'OWASP-ZAP'}
    }
    stage('Check XSS with Gauntlt'){
      steps {build 'Gauntlt-XSS-Attack'}
    }
  }
}

