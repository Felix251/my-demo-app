pipeline {
  agent any
  stages {
    stage(' dependencies') {
            steps {
                sh 'node -e "console.log(require(\'child_process\').execSync(\'npm -v\').toString())"'
                sh 'node -e "console.log(require(\'child_process\').execSync(\'npm install\').toString())"'
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
