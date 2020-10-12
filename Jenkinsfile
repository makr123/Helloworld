pipeline {
    agent any
    stages {
        stage('Example Build') {
            steps {
                echo 'Hello, Maven'
            }
        }
        stage('Example Test') {
            steps {
                cleanWs disableDeferredWipeout: true, deleteDirs: true
            }
        }
    }
}
