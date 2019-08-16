pipeline {
  agent { docker { image 'python:3.6' } }
  stages {
    stage('build') {
      steps {
        sh 'pip install -r Requirements.txt'
      }
    }
    stage('test') {
      steps {
        sh 'python app.py'
      }  
    }
  }
}
