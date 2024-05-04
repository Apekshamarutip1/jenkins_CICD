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
          emailext body: 'Success', subject: 'Testmail for first jenkins job', to: 'apputest250@gmail.com'
      }
}
}
