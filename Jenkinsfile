pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    sh 'g++ -o PES1UG22CS641-1.cpp' // Compile the C++ file
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    sh './output' // Run the compiled executable
                }
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the application...' // Modify this step based on deployment needs
            }
        }
    }

    post {
        failure {
            echo 'Pipeline failed!'
        }
    }
}
