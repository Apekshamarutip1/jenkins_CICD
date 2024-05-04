pipeline {
  agent any
  stages {
    stage('Build') { 
            steps { 
                echo "build stage" 
            }
        }
    stage('Test') {
      steps {
             echo "Test stage"
      }
    }
  }
  post {
        always {
            emailext( body: 'A Test EMail', 
               subject: 'Test'
               to: 'apputest250@gmail.com'      
                     )
        }
    }
}
