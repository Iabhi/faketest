pipeline {
    agent none
    stages {
		stage('First stage'){
			steps('Input') {
				Input {
					message "Your name..."
					ok'submit'
					parameters {
						// A simple text input
						string(name: 'PERSON', defaultValue: 'Mr Biswas', description: 'Who should I say hello to?')
					}
            }
        
		
        options{
            timeout(time:10,unit:'SECONDS')
        }
		
        
        steps {
                echo "Testing.."
                sh '''
                echo 'Abhishek! HelloWorld!'
                '''
            }
			}		
		}
	}
}
