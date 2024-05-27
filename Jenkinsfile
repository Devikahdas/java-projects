pipeline{
  agent none
    stages{
      stage('FRont-end'){
        agent{
          docker{ image 'maven:3.8.1-adoptopenjdk-11'}
        }
        steps{
          sh 'mvn --version'
        }
      }
      stage('Back-end'){
        agent{
          docker{image 'node:16-alpine'}
        }
        steps{
          sh 'node --version'
        }
      }
    }      
}
