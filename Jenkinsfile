pipeline {
  agent {
    docker {
      image 'williamyeh/ansible'
      args 'ubuntu14.04'
    }
    
  }
  stages {
    stage('checkout') {
      steps {
        dir(path: 'release') {
          git(url: 'https://github.com/goblin23/chef-spring-boot.git', branch: 'master', credentialsId: 'b59ef31f-482f-4ff4-a787-e552c9f89396')
        }
        
      }
    }
  }
}