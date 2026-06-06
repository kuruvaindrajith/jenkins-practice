pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                sh 'exit 1'
            }
        }

    }

    post {

        always {
            echo 'Pipeline Finished'
        }

        success {
            echo 'Build Successful'
        }

        failure {
            echo 'Build Failed'
        }

    }
}
