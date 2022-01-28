pipeline {
    agent any

    tools {
        Maven "3.8.4"
    }
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