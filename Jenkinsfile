// * Groovy - Based off of Java Object language

pipeline {
    agent any // What node you're using, don't concern yourself about it

    environment {
        string = credentials('secretString')
        login = credentials('userPass')
    }

    stages { // What stages you're wanting jenkins to do
        stage('helloWorld') { // Define a stage of the CI/CD
            steps {
                sh 'echo "HelloWorld"'// Step, what you want it to do
                sh 'pwd' // Lists the path you're on
                sh 'ls'
                // sh 'cd /home/ubuntu/project' 
            }
        }

        stage('print secret data') {
            steps {
                sh 'echo ${string}'
                sh 'echo ${login}'
                sh 'echo ${login_USR}'
                sh 'echo ${login_PWD}'
            }
        } 
    }
}