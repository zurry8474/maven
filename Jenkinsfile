pipeline {
    agent any 
    stages {
        stage("Builds in maven") {
            steps{
                sh "mvn -version"
                sh "mvn clean install"
            
            }
        }
    }

    post{
        always{
            cleanWs()
        }
    }

}