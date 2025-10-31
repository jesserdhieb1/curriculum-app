pipeline {
  agent any
  stages {
    stage('Install Deps') {
      steps {
        sh '''apt update && apt upgrade
apt install git'''
      }
    }

    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/jesserdhieb1/curriculum-app', branch: 'dev')
      }
    }

  }
}