pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'started!'
            }
        }

        stage('Check Files') {
            steps {
                sh 'ls -la'
                sh 'pwd'
            }
        }
    }
}
