pipeline {
	agent { docker { image 'maven:3.6.3'} }
	//agent { docker { image 'node:13.8'} }
	stages {
		stage('Build') {
			steps {
				sh "mvn --version"
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
