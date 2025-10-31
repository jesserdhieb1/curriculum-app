pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        sh 'git --version'
        git(url: 'https://github.com/jesserdhieb1/curriculum-app.git', branch: 'dev')
      }
    }

    stage('Check Content') {
      parallel {
        stage('Check Content ') {
          steps {
            sh 'ls -la'
          }
        }

        stage('Unit tests') {
          steps {
            sh '''node --version
npm --version
cd curriculum-front
npm ci
npm run test:unit'''
          }
        }

      }
    }

  }
}