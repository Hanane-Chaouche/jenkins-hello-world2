pipeline {
    agent any
    environment {
        JAVA_HOME = 'C:\\Program Files\\Java\\jdk-17' // ← Chemin vers ton Java 17
        PATH = "${JAVA_HOME}\\bin;${env.PATH}"
    }
    stages {
        stage('Build') {
            steps {
                script {
                    bat 'python hello.py'
                    bat 'javac HelloWorld.java && java HelloWorld'
                }
            }
        }
    }
}

