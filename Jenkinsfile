pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Hello Build'
                echo 'Hi Bhai'
            }
        }
        stage('Test') {
            steps {
                echo 'Hello Build'
                echo 'Hi Bhai'
            }
        }
        stage('Deployee') {
            steps {
                echo 'Hello Build'
                echo 'Hi Bhai'
            }
        }
    }
    
    post {
        always {
            echo 'This will always execute'
        }
        failure {
            echo 'This will only execute if there is a failure'
            emailext body: 'Bhai', subject: 'Hello', to: 'rahulgavane65@gmail.com'
        }
    }
}
