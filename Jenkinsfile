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
        branch "main"
      }
      steps {
        sh '''
        cat README.md
        '''
      }
    }

   }

}
