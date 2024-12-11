pipeline {
    agent any

    stages {
        stage("Prepare") {
            steps {
                echo "Start Job: ${env.JOB_NAME}"
                echo "Build Number: ${env.BUILD_NUMBER}"
                echo "Branch Name github: ${env.BRANCH_NAME}"
                echo "Author: ${env.AUTHOR}"
            }
        }
        stage("Build") {
            steps {
                echo "Start Build..."
            }
        }
        stage("Test") {
            steps {
                echo "Start Test..."
            }
        }
        stage("Deploy") {
            steps {
                echo "Start Deploy..."
            }
        }
    }

    post {
        always{
            echo "This will always run"
        }
        success{
            echo "This will run success"
        }
        failure{
            echo "This will run failure"
        }
        cleanup{
            echo "This will run cleanup"
        }
    }
}
