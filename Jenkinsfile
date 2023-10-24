//DeCLARATIVE

pipeline {
	agent any 
	//agent { docker { image 'maven:3.6.3'}}
	stages {
			stage('Build') { 
			steps { 
			//sh 'mvn --version'
			echo "Build"
			echo "PATH - $PATH"
			echo "BUILD_NUMBER - $env.BUILD_NMUMBER"
			echo "BUILD_ID - $env.BUILD_ID"
			echo "JOB_NAME - $env.JOB_NAME"
			echo "BUILD_TAG - $env.BUILD_TAG"
			}	
			}
		
		stage('Test'){
			steps {
				echo "Test"
			}
		}

		stage('Integration Test'){
			steps {
				echo "Integration Test"
					}
}
	}
	post {
		always {
			echo "Im awesome .I Run always"
		}
		success {
			echo "I run when you are successful"
		}
		failure {
			echo "Irun when you are fail"
		}
		}
}

	
	




