pipeline {
    agent any
    stages {
        stage('Example Build') {
            steps {
                echo 'Hello, Maven'
                sh 'mvn --version'
            }
        }
        stage('Example Test') {
            steps {
                cleanWs disableDeferredWipeout: true, deleteDirs: true
            }
        }
    }
}
