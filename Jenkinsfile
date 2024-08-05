pipeline {
  agent any	
  stages {
    
    stage ('BUILD') {
      steps {
        echo "This is Build stage" 
              }  
    }  
    
    stage ('TEST PARALLEL') {
      parallel {
        stage ('TEST ON CHROME') {
          steps {
        echo "This is Test on chrome" 
          }
        }

        stage ('TEST ON SAFARI') {
          steps {
        echo "This is Test on SAFARI" 
          }
        }
      }  
    }   
    
    stage ('DEPLOY') {
      steps {
        echo "This is Deploy stage" 
        
      }  
    }  
  } 

}
  

