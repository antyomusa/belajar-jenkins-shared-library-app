pipeline {
    agent none
    stages{
        stage("Prepare"){
            agent {
                node {
                    label "Linux && java17"
                }
            }
            steps{
                echo("Start Job : ${env.JOB_NAME}")
                echo("Start Build : ${env.BUILD_NUMBER}")
                echo("Branch Name : ${env.BRANCH_NAME}")
            }
        }

        stage("Build"){
            agent {
                node {
                    label "Linux && java17"
                }
            }
            steps{
                echo("Start Build")
                sh("mvn clean compile test-compile")
                echo("Finish Build")
            }
        }

        stage("Test"){
            agent {
                node {
                    label "Linux && java17"
                }
            }
            steps{
                echo("Start Test")
                sh("mvn test")
                echo("Finish Test")
            }
        }

        stage("Deploy"){
            agent {
                node {
                    label "Linux && java17"
                }
            }
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