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
        stage ('TEST1') {
          steps {
        echo "This is Test1" 
          }
        }

        stage ('TEST2') {
          steps {
        echo "This is Test2" 
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
      }
    }
        
      
        stage ('SERVER 2')  {
      steps {
        echo "This is Deploy to server2" 

      }
        }
         
        
    }  
  } 


  

