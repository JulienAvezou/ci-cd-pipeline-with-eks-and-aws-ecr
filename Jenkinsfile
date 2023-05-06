#!/usr/bin/env groovy

pipeline {
    agent any
    stages {
        stage('copy files to ansible server') {
            steps {
                script {
                    echo "copying necessary files to ansible control node"
                    sshagent(['ansible-server-key']) {
                       sh "scp -o StrictHostKeyChecking=no ansible/* root@161.35.194.49:/root"

                        withCredentials([sshUserPrivateKey(credentialsId: 'ec2-server-key', keyFileVariable: 'keyfile', usernameVariable: 'user')])
                        sh "scp ${keyfile} root@161.35.194.49:/root/ssh-key.pem"
                    }

                }
            }

        }

    }
}
