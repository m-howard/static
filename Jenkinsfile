pipeline {
  agent any
  
  stages {
    stage('Upload to AWS') {
      steps {
        withAWS(credentials:'aws-static') {
          s3Upload(file: 'index.html', bucket:'markus-devops-udacity-project4', path:'index.html')
        }
      }
    }
  }
}
