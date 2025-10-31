pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        sh 'git --version'
        git(url: 'https://github.com/jesserdhieb1/curriculum-app.git', branch: 'dev')
      }
    }

  }
}