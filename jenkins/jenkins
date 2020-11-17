pipeline {
    agent any

    Stage('Build') {
        step {
            sh 'python -m py_compile HelloPython.py'
        }
    }
}