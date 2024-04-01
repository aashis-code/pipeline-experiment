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
                
                bat 'javac ./Test.java'
            }
        }
        
        stage('run'){
            steps {
           
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
