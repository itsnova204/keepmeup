pipeline {
    agent any

    stages {
        stage('Deploy') {
            steps {
                echo 'Deploying....'


                sh 'pip3 install -r requirements.txt'
                sh 'python3 keepmeup/manage.py runserver'
            }
        }
    }
}