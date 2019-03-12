pipeline{
	agent any
	stages{
		stage('build'){
			steps {
				echo 'building'
			}
		}
		stage('test') {
			steps {
				echo 'testing'
			}
		}
		stage('Deploy'){
			steps {
				echo 'deploying.....'
			}
		}
		stage('example test') {
			when {
				not {
					branch "master"
				}
			}
			steps {
				echo "example testing..."
			}
		}
	}
}
