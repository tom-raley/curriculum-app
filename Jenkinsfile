pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/tom-raley/curriculum-app', branch: 'dev')
      }
    }

    stage('Log') {
      steps {
        steps {
          sh 'ls -la'
        }
      }
    }

    stage('Build') {
      steps {
        sh 'docker build -f curriculum-front/Dockerfile .'
      }
    }
  }
}