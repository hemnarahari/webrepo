pipeline {
   agent any
    stages {
	  stage ('Compile Stage') {
	   steps {
	    withMaven(maven: 'maven_3.5.3') {
	   
		sh 'mvn clean' 
		}
		}  
		}
		
		 stage ('Test Stage') {
	     steps {
	     withMaven(maven: 'maven_3.5.3') {
	       sh 'cd /var/lib/jenkins/workspace/pipeline job/simple_webapp/pom.xml'
		  sh 'mvn test'  
		}
		}  
		}
		 stage ('Deploy Stage') {
	     steps {
	      withMaven(maven: 'maven_3.5.3') {
	       sh 'cd /var/lib/jenkins/workspace/pipeline job/simple_webapp/pom.xml'
		  sh 'mvn install compile'
		}
		}  
		}
		}
		}
