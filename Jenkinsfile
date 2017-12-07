#!/usr/bin/env groovy

    [$class: 'GithubProjectProperty',
    displayName: '',
    projectUrlStr: 'https://github.com/Demo-pro/Sachin/']
    pipelineTriggers(upstream(
      threshold: 'SUCCESS',
      upstreamProjects: 'https://github.com/Demo-pro/Dravid/'
    ))

pipeline {
    agent any 

    stages {
        stage('Build') { 
            steps { 
                sh 'pwd' 
            }
        }
        stage('Test'){
            steps {
                sh 'java -version'
                
            }
        }
        stage('Deploy') {
            steps {
                sh 'ls'
                sh 'pwd'
            }
        }
    }
}
