pipeline {

    agent none

    stages {

        stage('Build') {
            agent{
                docker{
                    image 'python:2-alpine'
                }
            }
            steps {
                sh 'python HelloPython.py'
                stash(name: 'compiled-results', includes: 'sources/*.py*')
            }
        }
    }
}