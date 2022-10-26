pipeline {
    agent {label 'agent1'}
    // environment {
    //    dockerhub_cred = credentials('dockerhub')
    // }
    stages {
        stage('building docker image') {
            steps {
                sh 'docker build . node-app:$BUILD_TAG'
            }
        }
    //  stage('push image to dockerhub') {
    //         steps {
    //             sh 'doker tag node-app:$BUILD_TAG yossef/node-app:$BUILD_TAG'
    //             sh 'docker login -u ${docker_cred_USR} -p ${docker_cred_PSW}'
    //             sh 'docker push yossef/node-app:$BUILD_TAG'
    //         }
    //     }
    }
}
