//Scripted
// node {
// 		echo "Build"
	
// 		echo "Test"
	
// 		echo "Integration Test"
	
// }

//Declarative
pipeline {
	agent any
	stages {
		stage('Build') {
			steps {
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
			echo 'I will always run'
		}
		success {
			echo 'I run only when sucess'
		}
		failure {
			echo 'I run only when fail test polling'
		}
	}
}
