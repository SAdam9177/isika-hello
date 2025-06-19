pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo '-----====----- Connecting to GitHub -----====-----'
                git branch: 'main', url: 'https://github.com/SAdam9177/isika-hello.git'
            }
        }
      stage('Compile') {
            steps {
                echo '-----====----- Compiling Code -----====-----'
                bat 'javac *.java'
            }
        }
                stage('Run') {
            steps {
                echo '-----====----- Running Application -----====-----'
                bat 'java Hello'
            }
        }
    }
}
