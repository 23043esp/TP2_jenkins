pipeline {
    agent any
    stages {
	stage('Checkout') {
            steps {
                // Récupère le code depuis le dépôt GitHub
                git branch:'master',url:'https://github.com/23043esp/TP2_jenkins.git'
            }
        }
        stage('Compile') {
            steps {
                script {
                    // Compile le code Java
                    sh 'javac HelloWorld.java'

                }
            }
        }
        stage('Run') {
            steps {
                script {
                    // Exécute le code Java compilé
                    sh 'java HelloWorld'

                }
            }
        }
    }
}
