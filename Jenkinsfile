pipeline {
 agent any 
    tools {
       maven 'Maven' 
    }
    stages {
	  stage ('Compile Stage') {
	   steps {
	    
		   dir("/var/jenkins_home/workspace/Jenkins sample Java Maven Project/") {
		sh 'mvn clean compile' 
		   }	   
		}
		}  
		
		
		 stage ('Test Stage') {
	     steps {
	     
	     
		  dir("/var/jenkins_home/workspace/Jenkins sample Java Maven Project/") {
		sh 'mvn test' 
		   }	  
		
		}  
		}
		 stage ('Deploy Stage') {
	     steps {
	      
	      
		  dir("/var/jenkins_home/workspace/Jenkins sample Java Maven Project") {
		sh 'mvn install' 
		   }	  
		
		}  
		}
		}
		}
		
