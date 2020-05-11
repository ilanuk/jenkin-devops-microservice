//SCRIPTED

//DECLARATIVE
pipeline {
	// agent any
	agent {
		docker {
			//image 'maven:3.6.3'
			image 'node:13.8'
		}
	}
	stages {
		stage('Build') {
			steps {
				//sh 'mvn --version'
				sh 'node --version'
				echo "Build"
			}
		}
		stage('Test') {
			steps {
				echo "Test"
			}
		}
		stage('Integration Test') {
			steps {
				echo "Integration Test"
			}
		}
	}
	post {
		always {
			echo 'I am awesome. I always run'
		}
		success {
			echo 'I run when you are successfull'
		}
		failure {
			echo 'I run when you fail'
		}
		changed {
			echo 'changed'
		}
		unstable {
			echo 'unstable'
		}
	}
}