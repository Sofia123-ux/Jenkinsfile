pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'git@github.com:Sofia123-ux/18eleanningpipeline.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the project...'
                // sh './build.sh' або sh 'mvn package'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                // sh 'npm test' або sh 'pytest'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}
