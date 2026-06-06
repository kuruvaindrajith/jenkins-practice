pipeline {
    agent any

    parameters {
        choice(
            name: 'ENV',
            choices: ['dev', 'test', 'prod'],
            description: 'Select Environment'
        )
    }

    stages {

        stage('Build') {
            steps {
                echo "Building Application"
            }
        }

        stage('Deploy to PROD') {

            when {
                expression {
                    params.ENV == 'prod'
                }
            }

            steps {
                echo "Deploying to PROD Server"
            }
        }
    }
}
