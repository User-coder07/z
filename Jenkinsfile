pipeline{
    agent any
    environment{
        JAVA_HOME = "C://Program Files/Java/jdk-21"
        PATH ="${JAVA_HOME}\\bin;${env.PATH}"
    }
    stages{
        stage('cloning'){
            steps{
                git url: 'https://github.com/User-coder07/z.git',branch: 'main'
            }
        }
        stage("compile"){
            steps{
                bat 'javac Multiplication.java'
            }
        }
        stage('run java'){
            steps{
                bat 'java Multiplication'
            }
        }
    }
}
