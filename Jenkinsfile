pipeline {
	agent any
	//agent { docker { image 'maven:3.6.3'} }
	//agent { docker { image 'node:13.8'} }
	stages {
		stage('Build') {
			steps {
				//sh 'mvn --version'
				echo "Build"
				echo "PATH - $PATH"
				echo "BUILD_NUMBER -$env.BUILD_NUMBER"
				echo "BUILD__ID - $env.BUILD_ID"
				echo "JOB_NAME - $env.JOB_NAME"
				echo "BUILD_TAG - $env.BUILD_TAG"
				echo "BUILD_URL - $env.BUILD_URL"
			}
		}
	
	stage('Tester') {
		steps {
		echo "Test"
	}
	}
	stage('Integration Test') {
		steps {
		echo "Test"
	}
	   }
    } 
	post {
			   always {
				   echo 'Im awesome.I run always!'
			   }
			   success {
				   echo 'I run when you are succesful'
			   }
			   failure {
				   echo 'I ru  when you fail'
			   }
	}
		   
}
