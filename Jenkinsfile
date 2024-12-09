pipeline {
  environment {
        // Define environment variables for Docker, e.g., image name
        DOCKER_IMAGE = "myapp-image"
    
   }
  agent any
  stages {
    stage ('cloning git' ) {
      steps  {
        git branch: 'main', url: 'https://github.com/Syamkumar-18/Project1.git'
      }
    }
    stage ('Build Docker image') {
      steps {
          sh 'docker build -t sample-image .'
    }
    } 
  }
}
