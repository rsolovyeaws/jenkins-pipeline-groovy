def gv
pipeline { 
  agent any 
  
  stages{
    stage('Init') {
      steps { 
        script {
          gv = load "script.groovy"
        }
      }
    }
    stage('Build') {
      steps { 
        script { 
          gv.buildApp()
        }
      }
    }
    
    stage('Test') {
      steps { 
        echo "Test"
      }
    }
   
    stage('Deploy') {
      steps { 
        echo "Deploy"
      }
    }
  }
}
