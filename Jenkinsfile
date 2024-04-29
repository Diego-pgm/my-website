pipeline {
  agent any
  stages {
    stage('Build'){
      steps{
	sh '''
python3 -m venv $PWD 
. $PWD/bin/activate
python3 -m pip install -r requirements.txt'''
      }
    }
    stage('Deploy'){
      steps{
'''
echo 'This is the deployment step'
'''
      }
    }
  }
}
