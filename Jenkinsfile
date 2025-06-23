pipeline {
    agent {
        node {
            label "Linux && java17"
        }
    }
    stages{
        stage("Build"){
            steps{
                echo("Start Build")
                sh("mvn clean compile test-compile")
                echo("Finish Build")
            }
        }

        stage("Test"){
            steps{
                echo("Start Test")
                sh("mvn test")
                echo("Finish Test")
            }
        }

        stage("Deploy"){
            steps{
                echo("Hello Deploy 1")
                echo("Hello Deploy 2")
                echo("Hello Deploy 3")
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