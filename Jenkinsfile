pipeline {
	agent any
	parameters {
		choice(
			choices:['greeting','silence'],
			description: '',
			name:'Requsted_Action')
	}
	stages
		stage('Speak'){
			when{
				//only say hello if a "greeting" is requested
				expression { params.Requsted_Action == 'greeting'}
			}
			steps {
  				echo " Welcome to Harman!"
  			}
		}
	}
}
