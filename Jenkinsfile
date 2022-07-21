pipeline {
    agent any
environment {
    PATH="/opt/maven/bin:$PATH"
}
    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
         stage('Hi') {
            steps {
                echo 'Hoe are you '
            }
         }
stage('SCM'){
    steps{
         git 'https://github.com/Codng-4All/hello-world.git'
    }
    }
      stage('Build') {
            steps {
            sh"mvn package"
            }
         }    
