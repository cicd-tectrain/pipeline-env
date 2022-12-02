pipeline {
    agent any
    environment {
        NAME = 'Jenkins'
    }

    stages {
        stage('Use Environment') {
            steps {
                echo '${NAME}'
                echo "${NAME}"
            }
        }
    }

}