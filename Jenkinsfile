pipeline {
    agent {
        docker {
            image "maven:3.8.4-jdk-13"
            label "docker"
        }
    }
    stages {
        stage("Build") {
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