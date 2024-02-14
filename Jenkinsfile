pipeline {
  agent any
  stages {
    stage('checkout stage') {
      steps {
        sh 'rm -rf Tomcat_roles'
        sh 'git clone https://github.com/yatheesh2328/Tomcat_roles.git'
      }
    }
    stage('running playbook') {
      steps {
        sh 'ansible-playbook -i hosts tomcat_playbook.yml'
      }
    }
  }
}
