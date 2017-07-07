pipeline {
    agent { docker 'acleancoder/imagemagick-full' }
    stages {
        stage('build') {
            steps {
                sh 'sh threshold.sh 50 demo.jpg demp_threshold.gif'
            }
        }

    }
    

}
