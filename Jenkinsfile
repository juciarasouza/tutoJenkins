pipeline{
    agent {
        docker{
        image "ruby"
        }
    }
    stages {
        stage("build"){
            steps{
                sh "bundle install" 
            }
        }
        stage("test"){
            steps{
                sh "bundle exec cucumber -p ci"
            }
        }
    
    }
}
 