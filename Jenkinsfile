pipeline {
	agent any

	triggers {
		pollSCM('* * * * *')
	}
	
	stages {
		stage('Checkout') {
			steps {
				git 'https://github.com/POweNt/hello-jenkins.git'
			}	
		}

		stage('Build') {
			steps {
				sh 'mvn clean compile'
			}
		}
	
		stage('Run') {
			steps {
				sh 'java -cp target/classes Hello'
			}
		}	
	}
}
