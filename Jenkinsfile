pipeline {
  agent any
  stages {
    stage('Voting App Deploy') {
      parallel {
        stage('Get Sourses') {
          steps {
            git(url: 'https://github.com/haimkabesa/VotingSystem.git', branch: 'master')
          }
        }
        stage('Docker-Compose') {
          steps {
            sh '/usr/local/bin/docker-compose up -d'
          }
        }
      }
    }
  }
}