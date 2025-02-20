pipeline {
    agent any

    stages {
        stage("Build") {
            steps {
                sh "mvn compile"
            }
        }

        stage("Test") {
            steps {
<<<<<<< HEAD
                 wrap([$class: "Xvfb", debug: true, dispalyName: 11, displayNameOffset: 0, timeout:11]) {
=======
                wrap([$class: "Xvfb", debug: true, dispalyName: 11, displayNameOffset: 0, timeout:10]) {
>>>>>>> 98efd9200e42d5e189a986809ebb56108e505de5
                    sh "mvn test"
                }
            }
        }

        stage("Publish") {
            steps {
                testNG()
            }
        }
    }
}
