pipeline {
	agent any
	
	stages {
	    stage('Checkout') {
	        steps {
			checkout scm			       
		      }}
		stage('Build') {
	           steps {
			  sh '/home/prachi/Documents/devops-folder/apache-maven-3.9.3/bin/mvn install'
	                 }}
		stage('Deployment'){
		    steps {
			
		sh 'cp target/Flipkart5.war /home/prachi/Documents/devops-folder/apache-tomcat-9.0.76/webapps'
	}}
}}

