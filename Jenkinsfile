pipeline {
    agent any
    stages {
        stage('Build Code') {
            steps {
                sh "chmod u+x temp.py"
                sh "./temp.py"
            }
        }
    }
}
