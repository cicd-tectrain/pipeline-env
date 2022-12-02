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
                echo "${NAME}"
                sh 'echo ${CREDS}'
            }
        }
    }

}