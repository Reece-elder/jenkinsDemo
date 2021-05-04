// * Groovy - Based off of Java Object language

pipeline {
    agent any // What node you're using, don't concern yourself about it

    stages { // What stages you're wanting jenkins to do
        stage('helloWorld') { // Define a stage of the CI/CD
            steps {
                sh 'echo "HelloWorld"'// Step, what you want it to do
                sh 'pwd' // Lists the path you're on
                sh 'ls' 
            }
        } 
    }
}