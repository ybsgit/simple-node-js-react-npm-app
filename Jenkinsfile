pipeline{
    agent{
        docker{
            image 'node:14-alpine'
            args '-p 3000:3000'
            args '-u root:root'
        }
    }
    stages{
        stage('Build')
        {
            steps{
                sh 'npm install'
            }
        }
    }
}