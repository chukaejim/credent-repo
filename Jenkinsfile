pipeline {
    agent any

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
    }
}
