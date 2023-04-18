pipeline {
  agent any

  stages {
    stage('Build') {
      steps {
        sh 'docker build -t appexamen .'
      }
    }
    stage('Run') {
      steps {
        sh 'docker run -p 8081:80 -d appexamen'
      }
    }
  }
}
