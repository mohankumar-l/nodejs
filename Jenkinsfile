pipeline {
  agent any 
  stages {
        tools {nodejs "node"}
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
        sh 'node index.js &'
      }
    }
  }
}
