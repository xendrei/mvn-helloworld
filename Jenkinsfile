pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                sh "rm -rf *"
                sh "git clone https://github.com/xendrei/mvn-helloworld.git"
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
