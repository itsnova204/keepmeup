pipeline {
    agent any

    stages {
        stage('Deploy') {
            steps {
                echo 'Deploying....'

                sh 'virtualenv -p python3 kmu-venv'
                sh 'source kmu-venv/bin/activate'
                sh 'pip install -r requirements.txt'
                sh 'python keepmeup/manage.py runserver'
            }
        }
    }
}