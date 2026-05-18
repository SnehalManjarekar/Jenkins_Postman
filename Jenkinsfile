pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/SnehalManjarekar/Jenkins_Postman.git'
            }
        }

        stage('Install Newman') {
            steps {
                sh 'npm install -g newman'
            }
        }

        stage('Run Postman Tests') {
            steps {
                sh 'newman run Collection.json'
            }
        }
    }
}