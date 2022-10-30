pipeline {
    agent any

    stages {
        stage('Deploy') {
            steps {
                echo 'Deploying....'

                virtualenv -p python3 kmu-venv
                source kmu-venv/bin/activate
                pip install -r requirements.txt
                python manage.py runserver
            }
        }
    }
}