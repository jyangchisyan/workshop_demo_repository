pipeline {
    agent any
    stages {
        stage('Post Example') {
            steps{
                echo 'In stages'
            }
        }
    }
    post{
        always{
            echo 'after stage always execute it'
        }
        success{
            echo 'if job excute success, excute it'
        }
    }
}