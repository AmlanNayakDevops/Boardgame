pipeline {
    agent any
    
    tools {
        maven 'maven'
        jdk 'java 17'
    }

    stages {
        stage('new file') {
            steps {
                echo 'jenkins file'
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
   
    stage('test') {
            steps {
                sh 'mvn test'
            }
        }
    stage('package') {
            steps {
                sh 'mvn package'
            }
        } 
     stage('itsdone') {
            steps {
                echo 'its done'
            }
        }
    }
}
