pipeline{
    agent any
    stages{
        stage('checkout the code from github'){
            steps{
                 git url: 'https://github.com/Joice-ZZZ/Banking-java-project/'
                 echo 'github url checkout'
            }
        }
        stage('codecompile with joice'){
            steps{
                echo 'starting compiling'
                sh 'mvn compile'
            }
        }
        stage('codetesting with joice'){
            steps{
                sh 'mvn test'
            }
        }
        stage('qa with joice'){
            steps{
                sh 'mvn checkstyle:checkstyle'
            }
        }
        stage('package with joice'){
            steps{
                sh 'mvn package'
            }
        }
         
    }
}
