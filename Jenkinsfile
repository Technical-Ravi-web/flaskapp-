pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                git 'https://github.com/Technical-Ravi-web//FlaskApp.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'pip3 install -r requirements.txt'
            }
        }

        stage('Run App') {
            steps {
                sh 'nohup python3 app.py &'
            }
        }
    }
}
