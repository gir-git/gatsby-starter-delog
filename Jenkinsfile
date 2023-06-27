pipeline {
    agent any

    stages {
        //stage('Stage 1: Git Pull') {
          //  steps {
          //      echo 'going to pull code from github repo '
          //      sh 'git pull'
          //  }
        //}
        
        stage('Stage 2: Build') {
            steps {
                echo 'running "npm install && npm run build"'
                nodejs(nodeJSInstallationName: 'Node 20.3.1') {
                    sh 'npm config ls'
                    sh 'npm install'
                    sh 'npm run build'
                }
            }
        }
        
        stage('Stage 3: Deploy') {
            steps {
                echo 'running "npm run deploy"'
            }
        }
    }
}
