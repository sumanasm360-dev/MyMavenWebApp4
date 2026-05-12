pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/sumanasm360-dev/MyMavenWebApp4.git'
            }
        }

        stage('Build') {
            steps {
                sh 'echo "Build step here"'
            }
        }
    }

    post {
        success {
            echo 'Build successful'
        }
        failure {
            echo 'Build failed'
        }
    }
}
