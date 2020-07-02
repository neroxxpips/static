pipeline {
    agent any
    stages {
        stage('Upload to AWS') {
            steps {
                    withAWS(region:'us-east-1', credentials:'aws-static') {
                    // do something
                    }                 
                    s3Upload(file:'index.html', bucket:'neroxxpips-jenk', path:'static/index.html')
                    sh 'echo "Hello World"'
                    sh '''
                        echo "Multiline shell steps works too"
                        ls -lah
                    '''
            }
        }
    }
}
