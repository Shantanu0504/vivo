pipeline {
	agent any 
	
	triggers {
    '* * * * *'
}
	stages {
	    stage('Checkout') {
	        steps {
			checkout scm			       
		      }}
		stage('Build') {
	           steps {
			  sh '/home/shantanu/Downloads/Devops/apache-maven-3.9.5-bin/apache-maven-3.9.5/bin /mvn install'
	                 }}
		stage('Deployment'){
		   steps {
		sh 'cp target/vivo.war /home/shantanu/Downloads/Devops/apache-tomcat-9.0.82/webapps'
			}}	
}}
