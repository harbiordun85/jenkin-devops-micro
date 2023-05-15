pipeline {
  // agent { docker { image 'node:13.8'} }
  environment {
   dockerHome = tool 'myDocker'
   Path = "dockerHome/bin:$PATH"

  }
 stages {
   stage ('Build') {
      steps  {
        // sh 'node --version'
        sh 'rm -rf app_server'
        sh 'git clone https://github.com/petejades/app_server.git'
        echo "Build"
        echo "PATH - $PATH"
        echo "BUILD_NUMBER - $env.BUILD_NUMBER"
        echo "BUILD_NUMBER - $env.BUILD_NUMBER"
        echo "BUILD_ID - $env.BUILD_ID"
        echo "JOB_NAME - $env.JOB_NAME"
        echo "BUILD_TAG - $env.BUILD_TAG"
        ECHO "BUILD_URL - $env.BUILD_URL"

      }

    } 
	
  }
}