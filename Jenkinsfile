pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                withAWS(region:'us-east-2') {
                    s3Upload(file:'index.html', bucket:'tanmay-jenkins-project-2', path:'index.html')
                }
            }
        }
            
    }
    
}