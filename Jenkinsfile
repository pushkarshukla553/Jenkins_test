pipeline {
    agent any 

    stages {
        stage('Build') {
            steps {
                script {
                    // Simulating a build step
                    echo 'Building...'
                    echo 'This is code cloning'
                    git url: 'https://github.com/pushkarshukla553/Jenkins_test.git' branch: 'main'
                }
            }
        }
        
        stage('Test') {
            steps {
                script {
                    // Simulating a test step
                    echo 'Running tests...'
                }
            }
        }
        
        stage('Deploy') {
            steps {
                script {
                    // Simulating a deployment step
                    echo 'Hello World!'
                }
            }
        }
    }
}
