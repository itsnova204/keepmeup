pipeline {
    agent any

    stages {
        stage('Deploy') {
            steps {
                echo 'Deploying....'


                sh 'pip install -r requirements.txt'
                sh 'python3 keepmeup/manage.py runserver'
            }
        }
    }
}