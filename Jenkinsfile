pipeline {
    agent any
    stages {
    stage('bisect'){
        steps{
        sh 'git bisect start 46578439ab651402b8bde0cba09a877f63ac7eaf f12518c4d471c30d33a4d16126adbc7e6d563188'    
        }
    }  
    stage('mvn clean bisect'){
        steps{
        sh 'git bisect run mvn clean test'    
        }
    }  
  }
 }

