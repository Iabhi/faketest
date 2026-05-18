pipeline {
    agent none
    stages {
		stage('First stage'){
			steps('Input') {
				Input {
					message "Your name..."
					ok'submit'
					parameters{
						string(name:'Varity', defaultValue: 'iswasBiswas'),
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
