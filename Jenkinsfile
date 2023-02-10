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
        script { 
          gv.printTest()
        }
      }
    }
   
    stage('Deploy') {
      steps { 
        echo "Deploy"
      }
    }
  }
}
