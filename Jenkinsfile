pipeline{
    agent {
        docker{
        image "ruby"
        }
    }
    stages {
        stage("build"){
            steps{
                sh "echo 'simular'" 
            }
        }
        stage("test"){
            steps{
                sh "bundle exec cucumber -p ci"
            }
        }
    
    }
}
