
pipeline {
  agent any
  stages {
    stage('Upload to AWS') {
      steps {
        withAws(credentials:'aws-static', region: 'us-west-2'){
          s3Upload(file:'index.html', bucket: 'ydnstatic')
        }
      }
    }
  }
}
