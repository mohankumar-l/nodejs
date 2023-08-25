pipeline {
  agent any 
  stages {

    stage('Git') {
      steps {
		sh 'git clone https://github.com/mohankumar-l/nodejs.git'
      }
    }
     
    stage('Build') {
      steps {
        sh 'npm install'
      }
    }  
    
            
    stage('Test') {
      steps {
        sh 'nohup node index.js &'
      }
    }
}
