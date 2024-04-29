pipeline {
  agent any
  stages {
    stage('Build'){
      steps{
	sh 'pip3 install -r requirements.txt'
      }
    }
    stage('Deploy'){
      steps{
        sh 'python3 -m flask run --host=0.0.0.0'
      }
    }
  }
}
