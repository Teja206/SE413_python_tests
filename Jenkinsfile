pipeline {
		agent none
		stages {
				stage('Build') {
						agent {
								docker {
										image 'python:2-alpine'
								}
						}
						steps {
								sh 'python -m py_compile my_sum/__init__.py'
						}
				}
		}
}
