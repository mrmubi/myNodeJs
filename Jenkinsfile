pipeline { 
    agent any 
    stages {
        stage('Build') { 
            steps { 
                    sh 'npm config ls'
                 
            }
        }
        stage('Test'){
            steps {
                sh 'make check'
                junit 'reports/**/*.xml' 
            }
        }
    }
}
