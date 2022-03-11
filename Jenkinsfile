pipeline {
	agent any
		stages {
			stage('First') {
				steps {
					sh "echo 'Step One' "
					script {
							env.VARIABLE="true"
						}
				}
			}


			stage('Second') {
				when{
					allOf { branch 'main'; environment name: 'VARIABLE', value: 'true' }
					echo "${VARIABLE}"
					
						}
				steps {
					sh "echo 'Updating Second Stage' "
					
				}
			} 

			stage('Third') {
				steps {
					sh "echo 'Step Three'"
				}
			}
		}
}


