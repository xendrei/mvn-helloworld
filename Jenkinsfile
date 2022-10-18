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
                sh "cd mvn-helloworld"
                sh "mvn package"
            }
        }
        stage('Run') {
            steps {
                echo "Run"
            }
        }
    }
}
