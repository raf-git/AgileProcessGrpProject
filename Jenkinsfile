pipeline {
    agent any
    stages {
        stage('Build') {
            agent {
                docker {
                    image 'python:2-alpine'
                }
            }
            steps {
                sh 'python -m py_compile HelloPython.py'

                stash(name: 'compiled-results', includes: 'sources/*.py*')
            }
        }
    }
}