pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    // Simulating a build step
                    echo 'Building...'
                    echo 'This is code cloning'
                    git url: 'https://github.com/pushkarshukla553/Jenkins_test.git', branch: 'main'
                }
            }
        }

        stage('Dockerhub login') {
            steps {
                script {
                    // Use withCredentials to access Docker Hub credentials
                    withCredentials([usernamePassword(credentialsId: 'dockerhubcred', usernameVariable: 'DOCKER_USERNAME', passwordVariable: 'DOCKER_PASSWORD')]) {
                        // Login to Docker Hub
                        sh 'echo $DOCKER_PASSWORD | docker login -u $DOCKER_USERNAME --password-stdin'
                    }
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

