pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build'
            }
        }
       
        stage('Test') {
            steps {
                echo 'Test'
            }
        }
       
        stage('Deployee') {
            steps {
                echo 'Deployee'
            }
        }
    }
    post{
        always{
            emailext body: 'hi', subject: 'From Jenkins', to: 'rahulgavane65@gmail.com'
        }
        failure{
            echo "This will executes whem fails"
            emailext body: 'Fail', subject: 'From Jenkins fails', to: 'rahulgavane65@gmail.com'
        }
    }
}
