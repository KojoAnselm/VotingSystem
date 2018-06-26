pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Get Sourses') {
          steps {
            git(url: 'https://github.com/haimkabesa/VotingSystem.git', branch: 'master')
          }
        }
        stage('Info') {
          steps {
            sh '/usr/local/bin/docker-compose build'
          }
        }
      }
    }
  }
}