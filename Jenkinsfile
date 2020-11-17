pipeline {
    agent { docker { image 'python 3.9'}}
    stages {
        stage('build') {
            steps {
                //This sh step runs the Python command to compile your application and
                //its calc library into byte code files, which are placed into the sources workspace directory
                sh 'python HelloPython.py'
                //This stash step saves the Python source code and compiled byte code files from the sources
                //workspace directory for use in later stages.

            }
        }
    }
}