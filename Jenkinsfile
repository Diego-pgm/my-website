pipeline {
  agent any
  stages {
    stage('Build'){
      steps{
	sh '''
python3 -m venv $PWD 
source $PWD
python3 -m pip install -r requirements.txt

        '''
      }
    }
    stage('Deploy'){
      steps{
        sh 'python3 -m flask run --host=0.0.0.0'
      }
    }
  }
}
