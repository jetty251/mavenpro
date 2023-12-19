pipeline {
    agent any
    environment {
        PATH = "/opt/maven3.9.6/bin:$PATH"
    }
    stages {
        stage("Clone Code") {
            steps {
               git branch: "master", url: "https://github.com/jetty251/mavenpro.git"
            }
        }
        stage("Build Code") {
            steps {
                sh "mvn clean install"
            }
        }
     }
 }
