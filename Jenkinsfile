pipeline {
    agent any

    stages {
        stage('📥 Checkout') {
            steps {
                echo 'Code pull ho gaya!'
            }
        }

        stage('📦 Install Dependencies') {
            steps {
                bat 'npm install'
            }
        }

        stage('🔨 Build Project') {
            steps {
                bat 'npm run build'
            }
        }

        stage('🚀 Serve App') {
            steps {
                echo 'App live ho rahi hai localhost:5000 pe...'
                // 'serve' package se dist folder ko preview karenge
                bat 'npx serve -s dist -l 5000'
            }
        }
    }
}
