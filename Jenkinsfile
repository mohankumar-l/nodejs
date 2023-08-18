pipeline {
  agent any 
  stages {
        
    stage('Git') {
      steps {
		git 'https://github.com/mohankumar-l/nodejs.git'
      }
    }
     
    stage('Build') {
      steps {
        sh 'npm install'
      }
    }  
    
            
    stage('Test') {
      steps {
        sh 'node index.js &'
      }
    }
  }
}
