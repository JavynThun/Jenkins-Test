//Scripted
// node {
// 		echo "Build"
	
// 		echo "Test"
	
// 		echo "Integration Test"
	
// }

//Declarative
pipeline {
	agent any
	//agent {docker {image 'maven:3.6.3'}}
	stages {
		stage('Build') {
			steps {
				//sh "mvn --version"
				echo "Build"
				echo "$PATH"
				echo "BUILD_NUMBER - $env.BUILDNUMBER"
				echo "BUILD_ID - $env.BUILD_ID"
				echo "JOB_NAME - $env.JOB_NAME"
				echo "BUILD_TAG - $env.BUILD_TAG"
				echo "BUILD_URL - $env.BUILD_URL"

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
			echo 'I will always run'
		}
		success {
			echo 'I run only when sucess'
		}
		failure {
			echo 'I run only when fail'
		}
	}
}
