pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ pipeline.cpp'
                echo 'successful build!'
            }
        }
        stage('Test') {
            steps {
                sh './a.out'
                echo 'successful test!'
            }
        }
        stage('Deploy') {
            steps {
                echo 'success!'
            }
        }
    }
    post {
        failure {
           echo 'failed!'        
        }
    }
}
