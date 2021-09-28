pipeline {
    agent { dockerfile true }
    stages {
        stage('LinuxTweetApp') {
            steps {
                sh 'docker build -t linux_tweet_app .'
                sh 'docker container run --detach -p 80:80 linux_tweet_app'
            }
        }
    }
}
