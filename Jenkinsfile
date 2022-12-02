pipeline {
    agent any
    environment {
        NAME = 'Jenkins'
        CREDS = credentials('github_pat')
    }

    stages {
        stage('Use Environment') {
            steps {
                echo '${NAME}'
                echo "${NAME}" // User:Passwort
                sh 'echo ${CREDS}'
                sh 'echo ${CREDS} > secret.txt'
                sh 'cat secret.txt'
                // Es gibt 3 CREDS Variablen
                echo "${CREDS_USR}" // nur User
                echo "${CREDS_PSW}" // nur Passwort
            }
        }
    }

}