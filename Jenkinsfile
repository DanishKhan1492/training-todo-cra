pipeline {
    agent any
    parameters {
        string(name: 'PARAM1', description: 'Param 1?')
        string(name: 'PARAM2', description: 'Param 2?')
    }
    stages {
        stage('Build') {
            steps {
                echo "${params}"
                echo "Building the project ${params.MYPARAM1}"
            }
        }
        stage('Test') {
            steps {
                echo "Testing the project"
            }
        }
        stage('Deploy') {
            steps {
                echo "Deploying the project ${params.MYPARAM2}"
            }
        }
    }
}