pipeline {
  agent any
  stages{
    stage('Build'){
      step{
        echo 'Running Jenkinsfile'
        sh './gradlew build  --no-daemon'
        archiveArtifacts artifact: 'dist/train.zip'
       }
     }
  }
}
