pipeline{
    agent any
    tools{
        maven 'maven'
    }
    stages{
        stage('git clone'){
            steps{
                git 'https://github.com/tanupooja2000/WebApplication.git'
            }
        }
        stage('validate'){
            steps{
                sh 'mvn validate'
            }
        }
        stage('compile'){
            steps{
                sh 'mvn compile'
            }
        }
        stage('package'){
            steps{
                sh 'mvn package'
            }
        }
        
    }
}
