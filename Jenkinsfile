pipeline {
   agent any
    tools {
        maven 'maven_3.5.3' 
    }
    stages {
	  stage ('Compile Stage') {
	   steps {
	    
	     sh 'cd /var/lib/jenkins/workspace/pipeline job/simple_webapp/pom.xml'
		sh 'mvn clean compile' 
		}
		}  
		
		
		 stage ('Test Stage') {
	     steps {
	     
	      sh 'cd /var/lib/jenkins/workspace/pipeline job/simple_webapp/pom.xml'
		  sh 'mvn test'  
		
		}  
		}
		 stage ('Deploy Stage') {
	     steps {
	      
	       sh 'cd /var/lib/jenkins/workspace/pipeline job/simple_webapp/pom.xml'
		  sh 'mvn install compile'
		
		}  
		}
		}
		}
		
