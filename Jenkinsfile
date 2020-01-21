pipeline {
  agent {
    docker {
      image 'alpine'
    }

  }
  stages {
    stage('Test echo') {
      steps {
        sh 'echo "Hello World"'
      }
    }

    stage('Test env vars') {
      steps {
        echo '$(FOO)'
      }
    }

  }
  environment {
    FOO = 'bar'
  }
}