pipeline {
    agent any

    tools {
        maven 'maven'
        jdk 'java 17'
    }

    stages {
        stage('New File') {
            steps {
                echo 'Jenkins file'
            }
        }
        stage('Git Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/AmlanNayakDevops/Boardgame.git'
            }
        }
        stage('Compile') {
            steps {
                sh 'mvn compile'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        stage('Package') {
            steps {
                sh 'mvn package'
            }
        }
        stage('Done') {
            steps {
                echo 'Pipeline execution completed.'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully.'
        }
        failure {
            echo 'Pipeline failed.'
        }
    }
}

                echo 'ecr'
            }
        }
    }
}
