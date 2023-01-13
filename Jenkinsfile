pipeline {
  agent any
  stages {
    stage('Checkout') {
            steps {
                sh 'node -v'
            }
        }
    stage('Install dependencies') {
            steps {
                sh 'npm install'
            }
        }
        stage('Build') {
            steps {
                sh 'npm run build'
            }
        }

    stage("Deploy"){
      steps {
        echo "Deploying the application....."
      }
    }
  }
}
