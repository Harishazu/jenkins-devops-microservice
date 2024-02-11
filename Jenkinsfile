pipeline {

	    // agent any

		agent { 
			docker { image 'maven:3.6.3'} 
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
				 echo 'When is our marriage'
			 }
			 failure {
				 echo 'Success or failure'
			 }
		}
	    
	}

