pipeline {
 agent any 
    tools {
       maven 'maven' 
    }
    stages {
	  stage ('Compile Stage') {
	   steps {
	    
		   dir("/var/lib/jenkins/workspace/pipeline job/simple_webapp/") {
		sh 'mvn clean compile' 
		   }	   
		}
		}  
		
		
		 stage ('Test Stage') {
	     steps {
	     
	     
		  dir("/var/lib/jenkins/workspace/pipeline job/simple_webapp/") {
		sh 'mvn test' 
		   }	  
		
		}  
		}
		 stage ('Deploy Stage') {
	     steps {
	      
	      
		  dir("/var/lib/jenkins/workspace/pipeline job/simple_webapp/") {
		sh 'mvn install' 
		   }	  
		
		}  
		}
		}
		}
		
