pipeline{
    agent any
    stages{
        stage('Build'){
        //     steps{
        //         sh 'echo "Hello World"'
        //         sh '''
        //             echo "Multiline steps work too"
        //             ls -lah
        //         '''
        //     }
        // }
            withAWS(region:'us-east-2', ) {
                    s3Upload(file:'index.html', bucket:'tanmay-jenkins-project-2', path:'index.html')
                }
        }
    }
}