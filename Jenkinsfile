pipeline {
    agent any

    stages {
        stage('Clone') {
    steps {
        git branch: 'main', url: 'https://github.com/Izzul27/learn-jenkins.git'
    }
}

        stage('Build') {
            steps {
                sh 'echo "Build success"'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                mkdir -p /var/www/laravel
                cp -r * /var/www/laravel
                '''
            }
        }
    }
}
