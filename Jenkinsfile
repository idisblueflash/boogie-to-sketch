pipeline {
    agent { docker 'python:3.5' }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
            }
        }

	stage('test') {
		      steps {
		      	    sh 'echo "a fake tat"'
		      }
	}
	    
	stage('Deploy') {
		steps {
			echo 'Deploying'
		}
	}
    }
    

}
