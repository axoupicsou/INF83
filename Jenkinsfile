pipeline {
  agent any

  stages {
    stage('Checkout') {
      steps {
        checkout scm
      }
    }

    stage('Build Docker Image') {
      steps {
        sh 'docker build -t node-ci-test .'
      }
    }

    stage('Run Tests') {
      steps {
        sh 'docker run --rm node-ci-test npm test || echo "Tests échoués"'
      }
    }

    stage('Simulated Deploy') {
      steps {
        echo 'Déploiement fictif effectué (ex: ssh ou rsync ici)'
      }
    }
  }
}
