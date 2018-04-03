pipeline {
   agent any
    tools {
        maven 'maven_3.5.3' 
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
	     
	     
		  sh 'mvn -f /var/lib/jenkins/workspace/pipeline job/simple_webapp/pom.xml test' 
		
		}  
		}
		 stage ('Deploy Stage') {
	     steps {
	      
	      
		  sh 'mvn -f /var/lib/jenkins/workspace/pipeline job/simple_webapp/pom.xml install'
		
		}  
		}
		}
		}
		
