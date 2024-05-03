pipeline {
  agent {
    docker { image 'node:16-alpine' }
  }
  stages {
    stage('Build') { 
            steps { 
                echo "build stage" 
            }
        }
    stage('Test') {
      steps {
        sh 'node --version'
      }
    }
  }
}
