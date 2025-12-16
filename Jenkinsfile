pipeline {
    agent {
        docker { image 'python:3.14' }
    }

    stages {
        stage('Build') {
            steps {
                // Get some code from a GitHub repository
                git branch: 'main', url: 'https://github.com/webromain/processus-tests'

                // Run Python
                sh "python main.py"
            }
        }
    }
}
