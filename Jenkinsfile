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
    post {
        cleanup {
            /* clean up our workspace */
            deleteDir()
            /* clean up tmp directory */
            dir("${workspace}@tmp") {
                deleteDir()
            }
            /* clean up script directory */
            dir("${workspace}@script") {
                deleteDir()
            }
        }
    }
}
