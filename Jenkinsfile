pipeline {
  agent any
  stages {
    stage('Get Sourses') {
      steps {
        git(url: 'https://github.com/haimkabesa/VotingSystem.git', branch: 'master')
        sh '/usr/local/bin/docker-compose build'
      }
    }
  }
}