pipeline {
    agent {label 'instance'}
    // tools {

    //     git "Default"
    // }
    
    stages {

        // stage('Preperation') {
        //     steps {
        //         // Get some code from a GitHub repository
        //         git 'https://github.com/yossefsameh/jenkins-and-docker.git'

        //     }
        // }
         stage('Print Branch name') {
            steps {
                    
                 echo "${env.GIT_BRANCH}"

            }
        }       
   
    //     stage('building docker image') {
    //         steps {
    //             sh 'docker build -f dockerfile . -t yossefsameh/node-app:$BUILD_TAG'
    //         }
    //     }
    //  stage('push image to dockerhub') {
    //         steps {
    //             //sh 'doker tag node-app:$BUILD_TAG yossef/node-app:$BUILD_TAG'
    //             sh 'docker run -d -p 4001:3000 yossefsameh/node-app:$BUILD_TAG'
    //         }
    //     }
    //      stage('Push on Docker Hub') {
    //         steps {
    //             withCredentials([usernamePassword(credentialsId: 'dockerhub', usernameVariable: 'USERNAME', passwordVariable: 'PASSWORD')]) {
                
    //             sh 'docker login -u ${USERNAME} -p ${PASSWORD}'
    //             sh 'docker push yossefsameh/node-app:$BUILD_TAG'
    //         }
    //         }
    //      }
    }
}
