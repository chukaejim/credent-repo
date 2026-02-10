pipeline {
    agent any

    stages {
        stage('Hello A') {
            steps {
                echo 'Hello World'
            }
        }

        stage('Run Linux Commands') {
            steps {
                // Using a shell script block
                sh '''
                    date
                    # Check if cal exists before running to avoid failure
                    if command -v cal >/dev/null 2>&1; then
                        cal
                    else
                        echo "cal command not found, skipping..."
                    fi
                '''
            }
        }
    }
}
