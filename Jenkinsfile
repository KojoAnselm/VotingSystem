pipeline {
  agent any
  stages {
    stage('Get Sourses') {
      steps {
        git(url: 'https://github.com/haimkabesa/VotingSystem.git', branch: 'master')
        sh 'docker-compose build'
      }
    }
  }
}