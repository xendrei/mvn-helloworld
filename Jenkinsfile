pipeline {
    agent { label 'docker-slave' }

    stages {
        stage('Info') {
            steps {
                echo "Build number : ${env.BUILD_ID}"
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
