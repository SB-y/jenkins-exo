pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Début du build...'
            }
        }

        stage('Test') {
            steps {
                script {
                    if (fileExists('index.html')) {
                        echo 'index.html est présent.'
                    } else {
                        error 'index.html est manquant !'
                    }
                }
            }
        }
    }
}