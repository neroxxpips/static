pipeline {
    agent any
    stages {
        stage('Upload to AWS') {
            steps {
                    withAWS(region:'us-east-1') {
                    // do something
                    }
                    withAWS(Access Key ID : 'AKIAU2ZOFEXMVD7YXMIN', Secret Access Key : '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') {
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
