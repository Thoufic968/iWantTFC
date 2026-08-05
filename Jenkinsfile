pipeline {

    agent any

    stages {

        stage('Build Repo A') {
            steps {
                echo "Building Repo A"
            }
        }

    }

    post {

        success {
            build job: 'repo-b-pipeline',
                  wait: false
        }

    }
}
