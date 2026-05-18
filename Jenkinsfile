pipeline {
    agent any

    stages {

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

