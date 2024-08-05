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
      parallel {
        stage ('SERVER 1')  {
      steps {
        echo "This is Deploy to server1" 

      }
        }
        
       parallel {
        stage ('SERVER 2')  {
      steps {
        echo "This is Deploy to server2" 

      }
        }
         
      }  
    }  
  } 

}
  

