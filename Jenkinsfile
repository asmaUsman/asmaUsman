pipeline {
    agent any
    triggers {
        githubPush()
    }
      stages {
          stage('build') {
              steps {
                  echo 'Starting build and installing packages'
                  sh 'npm install'
              }
          }
          stage('start') {
              steps {
                  echo 'Start application'
                  sh 'npm start'
              }
          }
    }
}
