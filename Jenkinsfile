pipeline {
    agent any
    stages {
        stage('Upload to AWS') {
              steps {
                  withAWS(region:'us-east-1',credentials:'aws-static') {
                  sh 'echo "Uploading content with AWS creds"'
                      s3Upload(file:'index.html', bucket:'wolasjenkins', path:'C:/Users/Wola/Desktop/DevOps/Udacity/Cloud DevOps Engineer/jenkins/static/index.html')
                }
            }
        }
    }
}