@Library("belajar-jenkins-shared-library@main") _

mavenPipeline()

// import antyomusa.jenkins.Output;
//
// pipeline {
//     agent any
//     stages {
//         stage("Library Resources") {
//             steps {
//                 script {
//                     def config = libraryResource("config/build.json")
//                     echo(config)
//                 }
//             }
//         }
//         stage("Hello Person") {
//             steps {
//                 script {
//                     hello.person([
//                         firstName: "Anton",
//                         lastName: "Yoab"
//                     ])
//                 }
//             }
//         }
//         stage("Maven Build") {
//             steps {
//                 script {
//                     maven(["clean", "compile", "test"])
//                 }
//             }
//         }
//         stage("Global Variable") {
//             steps {
//                 script {
//                     echo(author())
//                     echo(author.name())
//                     echo(author.channel())
//                 }
//             }
//         }
//         stage("Hello Groovy") {
//             steps {
//                 script {
//                     Output.hello(this, "Groovy")
//                 }
//             }
//         }
//         stage("Hello World") {
//             steps {
//                 script {
//                     hello.world()
//                 }
//             }
//         }
//     }
// }