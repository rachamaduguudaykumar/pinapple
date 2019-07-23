pipeline {
    agent { label 'master' }
    stages {
        stage('git_clone_demo') {
            steps {
                echo 'Hello world!'
                git credentialsId: '7175bbf1-850b-4fe3-b6de-f5f97f7a3f96', url: 'https://github.com/rachamaduguudaykumar/pinapple.git'
            }
        }
    stage('Build') {
        steps {
            echo 'helloword'
            sh '''
            mvn clean
            mvn compile
            mvn test
            mvn package
            '''
        }
    }
    stage('Unittests') {
        steps {
            echo 'helloword'
        }
    }
    stage('sonar') {
        steps {
            echo 'helloword'
        }
    }
    stage('artifactory') {
        steps {
            echo 'helloword'
        }
    }
    stage('deploy') {
        steps {
            echo 'helloword'
        }
    }
    }
}
