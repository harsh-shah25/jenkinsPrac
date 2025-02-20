pipeline { 
agent any
    stages {
        stage('Clone Git') { /*you can also specify git location */
            steps {
                git 'https://github.com/harsh-shah25/jenkinsPrac.git'
            }
        }
        stage('Build Code') {
            steps {
                sh "chmod u+x temp.py"
                sh "./temp.py"
            }
        }

        // stage('Test Code') {
        //     steps {
        //         sh "chmod u+x Test.py"
        //         sh "./Test.py"
        //     }
        // }
    }
}
