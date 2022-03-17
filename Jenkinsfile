println "Executing from Jenkinsfile in carina-demo repository"
pipeline {
  agent any
  tools {
   maven 'mvn 3.8.4'
   jdk 'java 11'
        }
  stages {
    stage("Build"){
        steps{
            git 'https://github.com/PavelLyutov/TestingJenkins.git'
                   bat 'mvn clean compile'
        }
    }
    stage("Unit Test"){
        steps{
       
                           bat 'mvn clean verify'
           
        }
    }

     }
  }
