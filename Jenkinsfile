//DeCLARATIVE

pipeline{
	//agent any 
	agent { docker {image 'maven:3.6.3'}}
	stages{
		steps{
				sh 'mvn --version'
				echo "Build"
			}	
		
		}
		stage('Test'){
			steps{
				echo "Test"
			}
		}
		stage('Integration Test'){
			steps{
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

