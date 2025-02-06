pipeline {
  agent any
  stages {
    stage ('checkout') {
      checkout scmGit(branches: [[name: '**']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/Sukrutha24/nms.git']])
    }
    stage ('code analysis') {
      echo "code analysis complete"
    }
    stage ('build') {
      sh 'mvn clean package'
    }
  }
}

                                                                                     
