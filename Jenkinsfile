pipeline {
  agent any
  // agent { docker { image 'maven:3.6.3'} }
  // agent { docker { image 'node:13.8'} }
  environment {
   dockerHome = tool 'myDocker'
   PATH = "$dockerHome/bin:$mavenHome/bin$PATH"

  }
 stages {
   stage ('Build') {
      steps  {
        sh 'docker version'
        sh 'rm -rf app_server'
        sh 'git clone https://github.com/petejades/app_server.git'
        echo "Build"
        echo "PATH - $PATH"
        echo "BUILD_NUMBER - $env.BUILD_NUMBER"
        echo "BUILD_NUMBER - $env.BUILD_NUMBER"
        echo "BUILD_ID - $env.BUILD_ID"
        echo "JOB_NAME - $env.JOB_NAME"
        echo "BUILD_TAG - $env.BUILD_TAG"
        echo "BUILD_URL - $env.BUILD_URL"

      }

    } 
	
  }
}
