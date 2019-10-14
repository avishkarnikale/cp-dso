pipeline {
  agent any 
  stages {
    stage('Check secrets'){
        build 'Git-Secrets'
    }
    stage('Check dependencies'){
        build 'OWASP-DEP-CHECK'
    }
    stage('Check XSS with ZAP'){
        build 'OWASP-ZAP'
    }
    stage('Check XSS with Gauntlt'){
        build 'Gauntlt-XSS-Attack'
    }
  }
}

