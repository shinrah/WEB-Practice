pipeline {
    agent any

    stages {
        stage('crate a web dir') {
            steps {
                parameters {
                    string defaultValue: 'sergui', description: 'author of web application deploy', name: 'Author'
                    string defaultValue: 'Development', description: 'Environment to deploy', name: 'Environment'
                }
            }

            steps {
                echo "the responsible of this project is ${Author} and will be deploy ${Environment}"
                sh 'rm -rf /home/jenkins/web'
                sh 'mkdir /home/jenkins/web'
            }
        }
    }
}
