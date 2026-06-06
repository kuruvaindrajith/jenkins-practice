pipeline {
    agent any

    parameters {
        booleanParam(
            name: 'RUN_TESTS',
            defaultValue: true,
            description: 'Run Test Stage'
        )
    }

    stages {

        stage('Build') {
            steps {
                echo "Building Application"
            }
        }

        stage('Test') {

            when {
                expression {
                    params.RUN_TESTS
                }
            }

            steps {
                echo "Running Tests"
            }
        }
    }
}
