pipeline {
    agent any
    stages {
        stage("Build"){
            steps {
                sh '''
                    echo "Hello world"
                '''
            }
        }

        stage("Test") {
            when {
                branch "fix-*"
            }
            steps {
                sh "cat README.md"
            }
        }
    }
}