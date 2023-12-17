// @Library('roboshop-shared-library@main') _

pipeline {
    agent any 
    stages {
        stage('Lint Checks') {
            steps {
                //  script {
                //     sample.info()
                // }
                sh "echo Installing JSLint"
                sh "npm install jslint"
                sh "echo Starting lint checks"
                sh "node_modules/.bin/jslint.js server.js || true"
                sh "echo Lint checks completed"
            }
        }
        stage('Generating Artifacts') {
            steps {
                sh "echo Generating Artifacts*********"
                sh "npm install && ls -ltr"
            }
        }
    }
}
