pipeline {
    agent { docker 'python:3.5' }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
		sh '''
		   echo "Multiline shell steps works too"
		   ls -lah
		'''
            }
        }

	stage('test') {
		      steps {
		      	    sh 'echo "a fake tat"'
		      }
	}
    }
    
    post {
    	always {
		archive 'build/libs/**/*.jar'
		junit 'build/reports/**/*.xml'
	}
    }

}
