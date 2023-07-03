pipeline {
    agent any
    stages {
        stage("Create artifacts or make changes") {
            steps {
                sh "mkdir testfile"
                sh "git add testfile"
                sh "git commit -m 'Add testfile from Jenkins Pipeline'"
            }
        }
        stage("Push to Git Repository") {
            steps {
             
                    sh "git push -u origin main"
                
            }
        }
    }

}
