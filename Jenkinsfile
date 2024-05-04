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
      post {
     success {
          emailext body: 'Test stage Success', subject: 'Testmail for first jenkins job', to: 'apputest250@gmail.com'
      }
    }
  }
}
 post {
     always {
          emailext attachLog: true, body: 'Success', subject: 'Pipeline status: $BUILD_NUMBER ', to: 'apputest250@gmail.com'
      }
    }
  }
