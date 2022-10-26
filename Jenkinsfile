pipeline {
    agent {label 'master'}

    stages {
        
        // stage('Git') {
        //     steps {
        //         git 'https://github.com/yossefsameh/jenkins-and-docker.git'
        //     }
        // }
        
        stage('building docker image') {
            steps {
                sh 'docker build -f dockerfile . -t node-app:$BUILD_TAG'
            }
        }
     stage('push image to dockerhub') {
            steps {
                //sh 'doker tag node-app:$BUILD_TAG yossef/node-app:$BUILD_TAG'
                sh 'docker run -d -p 4000:3000 node-app:$BUILD_TAG'
            }
        }
    }
}
