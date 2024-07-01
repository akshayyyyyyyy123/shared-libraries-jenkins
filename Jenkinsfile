@Library('simple-shared-lib') _

pipeline {
    agent any
    
    stages {
        stage('Hello world') {
            steps {
                helloWorld()
                echo 'stage-1 over'
            }
        }
        stage('Welcome') {
            steps {
                script {
                    welcome.call('Akshay', 'SDE-1')
                    welcome.call('Abhishek', 'SWE-1')
                }
                echo 'stage-2 over'
            }
        }
        stage('Calculate') {
            steps {
                script {
                    calculate.add(1, 2)
                    calculate.sub(4, 2)
                }
                echo 'stage-3 over'
            }
        }
    }
}
