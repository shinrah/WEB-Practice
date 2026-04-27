pipeline {
    agent any

    parameters {
        string defaultValue: 'sergui', description: 'author of web application deploy', name: 'Author'
        string defaultValue: 'Development', description: 'Environment to deploy', name: 'Environment'
    }

    stages {
        stage('crate a web dir') {
            steps {
                sh 'rm -rf /home/jenkins/web'
                sh 'mkdir /home/jenkins/web'
            }
        }
    }
}
