pipeline {
    // Exécuter sur l'agent disponible (le serveur Jenkins)
    agent any

    stages {
        // Étape 1 : récupérer le code depuis le dépôt Git configuré dans le job
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        // Étape 2 : compiler le projet avec Maven
        stage('Compile') {
            steps {
                sh 'mvn compile'
            }
        }
    }
}
