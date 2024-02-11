pipeline {

	    // agent any

		agent any
	    stages {
			stage ('Build') {
				steps {
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

