pipeline {
    agent any

    stages {
        stage("GIT CLONE") {

            steps {
                git  branch: "master", url: 'https://github.com/nasutionam/pipeline-github.git'
            }
        }
        stage("Manual Approval") {
            steps {
                 input "Deploy to prod?"
            }
        }

        stage("Deploy To EC2") {
            steps {
                pwd
            }
        }
    }
}
