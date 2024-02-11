pipeline {

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
				 echo 'When is our marriage'
			 }
			 failure {
				 echo 'Success or failure'
			 }
		}
	    
	}

