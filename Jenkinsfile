pipeline {
    agent { docker 'python:2-alpine' }
    stages {
        stage('Build') {
            steps {
                echo 'Building'
                sh 'cp LICENSE LICENSE.bak'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing'
                sh 'test -e LICENSE.bak'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying'
            }
        }
    }
}
