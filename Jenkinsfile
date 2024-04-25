pipeline {
     agent any

     stages {
        stage('Verficar tools') {
            steps {
                sh 'docker info'
            }
        }
         stage('Build docker') {
            steps {
                sh 'docker build -t app-jenkins .'
            }
        }

        stage('Run docker') {
            steps {
                sh 'docker run -dit --name app-jenkins app-jenkins'
            }
        }

        stage('Run specs') {
            steps {
                sh 'docker exec app-jenkins ./vendor/bin/phpunit tests'
            }
        }

     }

}