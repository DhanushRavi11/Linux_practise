pipeline{
 agent any
 tools{
  maven 'maven'
  jdk 'java-11'
 }
 stages{
  stage('Git checkout'){
   steps{
    git branch: 'main', url: 'https://github.com/DhanushRavi11/Linux_practise.git'

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
