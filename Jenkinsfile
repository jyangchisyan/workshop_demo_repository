pipeline {
    agent any
    stages {
        stage('When return true Example') {
            when {
                expression{
                    return true
                }
            }
            steps { 
                echo "When return true!"
            }
        }  
        stage('When return false Example') {
            when {
                expression{
                    return false
                }
            }
            steps { 
                echo "When return false!"
            }
        }  
        stage('Script Example') {
            steps { 
                script {
                    if(true){
                        echo "script if true"
                    }
                    if(false){
                        echo "script if false"
                    }
                }
            }
        }  

    }
}