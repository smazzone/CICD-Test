pipeline {
   agent any

   stages {
      stage('Build') {
        steps {
          echo 'Building...'
          echo "Running ${env.BUILD_ID} ${env.BUILD_DISPLAY_NAME} on node ${env.NODE_NAME} and job ${env.JOB_NAME}"
        }
   }
   stage('Test') {
     steps {
        echo 'Testing...'
     }
   }
   stage('Deploy') {
     steps {
       echo 'Deploying on Staging...'
     }
     steps {
       echo 'Deploying on Integration...'
     }     
     steps {
       echo 'Deploying on QA...'
     }          
   }
  }
}
