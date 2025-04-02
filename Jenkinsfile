pipeline{
    agent any
        tools{
            jdk 'jdk17'
            maven 'maven'
        }
        stages{
            stage('Build Maven'){
                steps{
                    checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url:'https://github.com/DeepikaMTT/Devops.git']])
                    bat 'mvn clean install'
                }
            }
           
        }
}