pipeline {
    agent any

    stages {
        stage('Info') {
            steps {
                echo "${env.BUILD_ID}"
            }
        }
        stage('Build') {
            steps {
                sh "mvn package"
            }
        }
        stage('Run') {
            steps {
                sh "java -jar target/helloworld-app-1.0-SNAPSHOT.jar"
            }
        }
    }
}
