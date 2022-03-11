pipeline {
	agent any
		stages {
			stage('First') {
				steps {
					sh "echo 'Step One'
					env.VARIABLE='true' "
				}
			}


			stage('Second') {
				steps {
					sh "echo 'Step Two'
					echo 'Updating Second Stage' "
				}
			} 

			stage('Third') {
				steps {
					sh "echo 'Step Three'"
				}
			}
		}
}


