pipeline { 
    agent any
    stages {
        stage('Clone Git') {
            steps {
                script {
                    checkout([
                        $class: 'GitSCM',
                        branches: [[name: '*/main']],
                        userRemoteConfigs: [[
                            url: 'https://github.com/harsh-shah25/jenkinsPrac.git',
                            credentialsId: '846ee163-c377-4a93-ac1a-6522f87328df'
                        ]]
                    ])
                }
            }
        }
        stage('Build Code') {
            steps {
                sh "chmod u+x temp.py"
                sh "./temp.py"
            }
        }
    }
}
