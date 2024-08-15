
//declarative

pipeline {
	agent any
	//agent { docker {image 'maven:3.6.3'}}
	//agent { docker {image 'node:22.6'}}
	stages {
		stage('Build') {
			steps {
				//echo 'mvn --version'
				//echo 'node --version'
				echo "Build"
				echo "PATH - $PATH"
				echo "BUILD_NUMBER - $env.BUILD_NUMBER"
				echo "BUILD_ID - $env.BUILD_ID"
				echo "JOB_NAME - $env.JOB_NAME"
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
			echo 'Im awesome. I run always'
		}
		success {
			echo 'I run when you are successful'
		}
		failure {
			echo 'I failed'
		}
	}
}
