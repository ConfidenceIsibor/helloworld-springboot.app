pipeline {
    agent any
    stages {
        stage('git clone') {
            steps {
                git branch: 'main', url: 'https://github.com/ConfidenceIsibor/helloworld-springboot.app.git'
            }
        }
        stage('Maven Test') {
            steps {
                bat 'mvn test'
            }
        }
        stage('Maven Build') {
            steps {
                bat 'mvn package'
            }
        }
        stage('Maven Deploy') {
            steps {
                echo "Deploy the war file to the server"
            }    
        }
    }
}


