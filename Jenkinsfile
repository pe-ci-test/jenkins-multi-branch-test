#!/usr/bin/env groovy

pipeline {
    agent any

    stages {
        stage('a') {
            agent {
                docker {
                    image 'node'
                }
            }
            steps {
                sh('echo "Hallo" > testfile1')
                sh('node --version')
            }
        }
    }
}
