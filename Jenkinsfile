pipeline {
    agent any
    environment {
        PATH = "/opt/maven/bin:$PATH"
    }
    stages {
        stage('git clone') {
            steps{
                git url : 'https://github.com/AshutoshMishra-16/sparkjava-war.git', branch: 'main'
            }
        }
        
        stage('build') {
            steps {
                sh 'mvn clean install'
            }
        }
    }
}
