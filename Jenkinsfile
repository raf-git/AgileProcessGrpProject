pipeline {

    agent any

    stages {

        stage('Build') {

            steps {
                sh 'python HelloPython.py'
                stash(name: 'compiled-results', includes: 'sources/*.py*')
            }
        }
    }
}