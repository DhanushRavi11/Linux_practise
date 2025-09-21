pipeline{
 agent any
 tools{
  maven 'maven'
  jdk 'java-11'
 }
 stages{
  stage('Git checkout'){
   steps{
    git branch: 'version-1', url: 'https://github.com/DhanushRavi11/Jenkins.git'

   }
  }

  stage('compile'){
   steps{
    sh "mvn compile"
   }
  }

  stage('build'){
   steps{
    sh "mvn package"
   }
  }
 }
}
