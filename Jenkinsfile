pipeline {

	    // agent any

		agent {
        dockerContainer ( image 'maven:3.6.3')
              }
	    stages {
			stage ('Build') {
				steps {
				   sh 'mvn --version'
                   echo "Build" 
				}
			}
				stage ('Test') {
				steps {
				   echo "Test"
	               
				}
			}
				stage ('Integration') {
				steps {
                echo "Integration Test"
				}
			}
		}
		
	    post { 
			always {
			  echo 'Im a bad ass'
			}
			 success {
				 echo 'Should start when Im a bad ass'
			 }
			 failure {
				 echo 'Success or failure'
			 }
		}
	    
	}

