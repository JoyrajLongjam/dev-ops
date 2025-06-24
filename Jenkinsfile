pipeline{
  agent any
  stages{
    stage('Checkout Code'){
      steps{
        git branch: 'main',url:'https://github.com/JoyrajLongjam/dev-ops.git'
      }
    }
    stage('Build'){
      steps{
        sh 'echo "Building the app"'
      }
    }
    stage('Test'){
      steps{
        bat 'echo "Running tests"'
      }
    }
    stage('Deploy'){
      steps{
        bat 'echo "deploying"'
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
