pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo '🎉 Pipeline chal gayi bhai! SCM se pull ho gaya!'
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
