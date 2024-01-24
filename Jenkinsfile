ipeline {
	agent any 
	parameters {
		choice(name: 'ENVIRONMENT', choices: ['QA','UAT'], description: 'Pick Environment value')
	}
	stages {
	    stage('Checkout') {
	        steps {
			checkout scm			       
		      }}
		stage('Build') {
	           steps {
			  sh '/home/abhilash/Documents/DevOps/tar/apache-tomcat-9.0.82/bin/mvn install'
	                 }}
		stage('Deployment'){
		   steps {
		sh 'cp target/CPCB1.war /home/abhilash/Documents/DevOps/tar/apache-tomcat-9.0.79/webapps'
			}}	
}}
