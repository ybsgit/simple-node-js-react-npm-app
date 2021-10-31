pipeline{
    agent{
        docker{
            image 'node:14-alpine'
            args '-p 3000:3000'
        }
    }
    stages{
        stage('Build')
        {
            steps{
                sh 'rm -rf /.npm'
                sh 'npm install'
            }
        }
    }
}