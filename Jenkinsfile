pipeline {
	agent any
		stages {
			stage('First') {
				steps {
					sh "echo 'Step One' "
					script {
						when { environment name: 'EXECUTE', value: 'true' }
					}
				}
			}


			stage('Second') {
				steps {
					sh "echo 'Step Two' echo 'Updating Second Stage' "
					script {
						echo ${EXECUTE}
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


