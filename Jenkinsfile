pipeline {
	agent any
	stages {
		stage('Both build and test') {
			parallel {
				stage('Build') { 
					steps {
						sh 'sleep 10; echo "This is a Build stage"'
					}
				}
				
				stage('Test'){
					steps {
						sh '''
							sleep 10
							echo "This is a Test stage"
						'''
					}
				}
			} 
		}
		stage('Deploy'){
			steps {
				sh '''
					sleep 5
					echo "This is a Deploy stage"
				'''
			}
		}
		
			
	}
}


