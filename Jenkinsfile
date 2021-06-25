pipeline {
  agent any
  stages {
    stage('Build Resources') {
      steps {
        sh 'bash build.sh'
        emailext(subject: 'Build Status', body: 'This is the build status of the current project', attachLog: true, from: 'howdybuddy01@gmail.com', to: 'sushan@moco.com.np')
      }
    }

    stage('Test') {
      steps {
        sh 'echo \'This is test part\''
      }
    }

    stage('Deploy') {
      steps {
        sh '''echo "Deploying"
'''
        sh 'echo "Deployment is complete"'
      }
    }

  }
}