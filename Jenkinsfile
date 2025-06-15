pipeline {
	agent any
	
	stages {

		stage('Compile') {
			steps {
				sh 'javac Hello.java'
			}
		}
	
		stage('Run') {
			steps {
				sh 'java Hello'
			}
		}	
	}
}
