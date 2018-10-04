pipeline {
    agent any
    stages {
        stage('Hello') {
            steps {
                print '### Hello, world!!'
                print '### This is branch ' + env.BRANCH_NAME
            }
        }
    }

    post {
        always {
            echo '### Post action'
            deleteDir()
        }
    }
}
