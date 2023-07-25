pipeline {
  agent { label "master" } 
  stages {
    stage('Hello'){
       steps {
         echo "Hello"
      }
    }
    stage('cat Readme'){
      when {
        branch "fix-*"
      }
      steps {
        sh '''
        cat README.md
        '''
      }
    }

   }

}
