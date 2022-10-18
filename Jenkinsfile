pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo "Don’t need to clone..."
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
