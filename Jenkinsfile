// * Groovy - Based off of Java

pipeline {
    agent any // What node you're using, just keep as agent any

    environment {
        dockerAccount = credentials('githubAccount')
    }

    stages {

        stage ('helloWorld') {
            steps {
                sh 'echo helloWorld'
                sh 'pwd'
                sh 'ls'
            }
        }

        stage ('Docker Push') {
            steps {
                sh "echo docker login $dockerAccount"
                sh "echo $dockerAccount_PSW"
                sh "echo $dockerAccount_USR"
                sh "echo docker push"
            }
        }

        stage ('Jenkins structure') {
            steps {
                sh "chmod +x ./scripts/test.sh"
                sh "cd /scripts"
                sh "ls"
                sh "./scripts/test.sh"
            }
        }
    }
}