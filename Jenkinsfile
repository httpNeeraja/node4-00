
pipeline{
    agent any
    tool {
        nodejs 'NodeJS'
    }

    stages {
        
        stage('Check Node'){
            steps {
                sh 'node --version'
                sh 'npm --version'
            }

        }

        stage('run'){
            steps {
                sh 'npm start'
            }
        }

    }
    post {
        always {
            cleanWs()
        }
    }
}