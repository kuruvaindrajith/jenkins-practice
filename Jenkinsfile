pipeline {
    agent any

    parameters {
        string(
            name: 'APP_VERSION',
            defaultValue: 'v1',
            description: 'Application Version'
        )
    }

    stages {

        stage('Build') {
            steps {
                echo "Building Version: ${params.APP_VERSION}"
            }
        }

        stage('Test') {
            steps {
                echo "Testing Version: ${params.APP_VERSION}"
            }
        }

    }
}
