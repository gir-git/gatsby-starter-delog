pipeline {
    agent any

    tools {nodejs "Nodejs 20.3.1"}

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
                    bat 'npm config ls'
                    bat 'npm install'
                    bat 'npm run build'
            }
        }
        
        stage('Stage 3: Deploy') {
            steps {
                echo 'running "npm run deploy"'
            }
        }
    }
}
