@Library('roboshop@main') _

pipeline {
    agent any 
    stages {
        stage('Lint Checks') {
            steps {
                script {
                    node.lintchecks()
                }
            }
        }
        stage('Generating Artifacts') {
             steps {
                 sh "echo Generating Artifacts"
                 sh "npm install"
            }
        }
    }
}
