pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/ameysonvadkar24/File-Encrypter.git'
            }
        }

        stage('Build') {
            steps {
                sh '''
                cd "Password Protection"
                mkdir -p build
                javac -d build src/*.java
                '''
            }
        }
    }
}
