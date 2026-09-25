pipeline {
    agent any

    stages {
        stage('📥 Checkout') {
            steps {
                echo 'Code GitHub se successfully pull ho gaya hai!'
            }
        }

        stage('📦 Install Dependencies') {
            steps {
                echo 'Installing npm packages...'
                // Windows ke liye 'bat' command use hoti hai
                bat 'npm install'
            }
        }

        stage('🔨 Build Project') {
            steps {
                echo 'Building Vite/React project...'
                bat 'npm run build'
            }
        }
    }

    post {
        success {
            echo '🎉 CONGRATS BHAI! React App successfully build ho gayi!'
        }
        failure {
            echo '❌ Build fail ho gaya! Check karo PC mein Node.js install hai ya nahi.'
        }
    }
}
