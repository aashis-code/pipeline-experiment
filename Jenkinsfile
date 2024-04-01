pipeline {
    agent any

    stages {
        stage('build') {
            steps {
                echo 'Building application'
            }
        }
        
        stage('compile'){
            steps {
                echo 'This step involves compiling java file to Class file(byte code).'
                bat 'javac Test.java'
            }
        }
        
        stage('run'){
            steps {
                echo 'This step finally run the program.'
                bat 'java Test'
            }
        }
    }

    post{

        always{
            echo 'After completion of stages, always runs.'
        }

        success{
             echo 'After completion of stages, success.'
        }

        failure{
             echo 'After failure in stages, Fail.'
        }
    }
    
}
