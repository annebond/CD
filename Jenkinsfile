pipeline {
  agent any
  stages {
    stage('Build & Test') {
      parallel {
        stage('Build') {
          steps {
            sleep 12
            sleep 1
          }
        }

        stage('Unit Test (JUnit)') {
          steps {
            sleep 1
          }
        }

      }
    }

    stage('Push to Repo') {
      steps {
        sleep 1
      }
    }

    stage('Deploy (Docker)') {
      parallel {
        stage('Deploy (Docker)') {
          steps {
            sleep 1
          }
        }

        stage('Migrate DB') {
          steps {
            sleep 1
          }
        }

      }
    }

    stage('Smoke Test') {
      steps {
        sleep 1
      }
    }

  }
}