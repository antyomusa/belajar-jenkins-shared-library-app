pipeline {
    agent {
        node {
            label "Linux && java17"
        }
    }
    stages{
        stage("Hello"){
            steps{
                echo("Hello Pipeline")
            }
        }
    }

    post {
        always {
            echo "I will always say Hello again"
        }
        success {
            echo "Success"
        }
        failure {
            echo "Oh no, Failure"
        }
        cleanup {
            echo "Dont't care success or not"
        }
    }
}