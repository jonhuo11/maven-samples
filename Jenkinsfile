pipeline {
  agent any
  tools {
    maven 'mvn'
    jdk 'jdk'
  }
  stages {
    stage('checkout') {
      steps {
        git(url: 'https://github.com/jonhuo11/maven-samples.git', branch: 'master')
      }
    }

    stage('run') {
      steps {
        sh 'mvn verify'
      }
    }

  }
}
