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
				steps {
					sh "echo 'Step Two' echo 'Updating Second Stage' "
					script {
						echo ${VARIABLE}
					}
				}
			} 

			stage('Third') {
				steps {
					sh "echo 'Step Three'"
				}
			}
		}
}


