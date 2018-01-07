pipeline {
    agent any
    stages {
        stage('Parallel Example') {
            parallel {
                stage('Vagrant Up on Node') {
                    agent {
                        label "node"
                    }
                    steps {
                        dir('vm_workspace'){
                            git branch: 'vagrant_workspace', url: 'https://github.com/jyangchisyan/workshop_demo_repository.git'
                            sh 'ls -a'
                        }
                    }
                }
                stage('Check Master workspace') {
                    steps {
                        sh "ls -a"
                    }
                }
            }
        }
    }
}