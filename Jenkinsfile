pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build Application'
            }
        }
            
             stage('Test') {
            steps {
                echo 'Test Application'
            }
             }
            
             stage('Deploy') {
            steps {
                echo 'Deploy Application'
            }
            
        }
    }
    post
    {
        always
        {
            emailext body: 'Just a simple hit', subject: 'PIPELINE STATUS TEST', to: 'tripta.sahni@geminisolutions.com'
        }
    }
}
