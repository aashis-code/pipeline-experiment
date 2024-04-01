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
                
                sh 'javac ./Test.java'
            }
        }
        
        stage('run'){
            steps {
           
                sh 'java Test'
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
