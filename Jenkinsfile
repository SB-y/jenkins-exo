pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Compilation du projet...'
                echo 'Packaging en cours...'
            }
        }

        stage('Test') {
            steps {
                echo 'Lancement des tests unitaires...'
                
                
                script {
                    if (fileExists('index.html')) {
                        echo 'Le fichier index.html est présent.'
                    } else {
                        error 'index.html est manquant !'
                    }
                }

                echo 'Lancement des tests d’intégration...'
                echo 'Génération du rapport de tests...'
            }
        }
    }
}