pipeline {
	agent any
	tools {
	maven 'Maven'
	}
	stages {
	stage ('Initialize') {
		steps {
		sh '''
			echo "PATH = ${PATH}"
			echo "M2_HOME = ${M2_HOME}"
		   '''
		}
	}

	STAGE ('Build') {
	steps {
	sh 'mvn clean package'
	}
	}

	
	}
}
