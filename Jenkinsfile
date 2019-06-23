pipeline{
    agent {
        docker{
        image "ruby:alpine"
        }
    }
    stages {
        stage("build"){
            steps{
                sh "chmod +x build/alpine.sh"
                sh "./build/alpine.sh"
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
 