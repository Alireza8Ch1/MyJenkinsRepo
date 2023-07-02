pipeline {
    
    agent any
    stages {
        stage("first stage"){
              options {
        timeout(time: 10, unit: 'SECONDS') 
    }
            steps{
                echo "first stage running!"
            }
        }
        stage('Example') {
            steps {
                input 'procceed??'
            }
        }
    }
    post { 
        always { 
            echo 'post section has been run'
        }
    }
}
