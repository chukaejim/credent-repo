pipeline {
    agent any
    environment { 
        LOVE = 'chuka'
    }

    stages {
        stage('Hello A') {
            steps {
                echo 'Hello World'
            }
        }
  stage('run linux command') {
            steps {
                sh """
                date
                cal
                """
            }
        }
   stage('calling default env variable') {
            steps {
                sh 'echo My build number id is $BUILD_ID'
                sh 'echo My real name is Ejim $LOVE'
            }
        }
    }
}
