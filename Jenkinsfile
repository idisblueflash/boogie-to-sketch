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
    }
    
    post {
    	always {
		archive 'build/libs/**/*.jar'
		junit 'build/reports/**/*.xml'
	}
    }

}
