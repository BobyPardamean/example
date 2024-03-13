pipeline {
    agent any

    stages {
        stage('Install Dependencies') {
            steps {
                script {
                    // Menginstal dependensi Node.js menggunakan npm
                    sh 'npm install'
                }
            }
        }

        stage('Build') {
            steps {
                script {
                    // Menjalankan proses build
                    sh 'npm run build'
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    // Menjalankan skrip pengujian
                    sh 'npm test'
                }
            }
        }

        stage('Deploy') {
            steps {
                script {
                    // Menjalankan proses deployment
                    sh 'npm run deploy'
                }
            }
        }
    }
}
