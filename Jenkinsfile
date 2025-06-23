pipeline{
  agent any
  stages{
    stage('Checkout Code'){
      steps{
        git 'https://github.com/JoyrajLongjam/dev-ops/new/main'
      }
    }
    stage('Build'){
      steps{
        sh 'echo "Building the app"'
      }
    }
    stage('Test'){
      steps{
        sh 'echo "Running Tests"'
      }
    }
    stage('Deploy'){
      steps{
        sh 'echo "deploying"'
      }
    }
  }
post{
  success{
    bat 'echo "build sucessful"'
  }
  failure{
    bat 'echo "build failed"'
  }
}
}
