pipeline {
  agent any
  stages {
    stage('State1') {
      parallel {
        stage('Stage1') {
          steps {
            sh 'echo " Parallel Step1"'
          }
        }
        stage('Step2') {
          steps {
            sh 'Echo "Parallel Step2"'
          }
        }
      }
    }
    stage('loop') {
      steps {
        sh '''for i in 1 2 3 4; 

do echo $i; done


'''
      }
    }
  }
}