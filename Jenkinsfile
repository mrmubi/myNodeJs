pipeline { 
    agent any 
    stages {
        stage('Build') { 
            steps { 
                 nodejs(nodeJSInstallationName: 'Node 11.3.0') {
                    sh 'npm config ls'
                 }
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
