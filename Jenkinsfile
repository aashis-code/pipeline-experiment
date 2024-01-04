pipeline {
    agent any

    stages {
        stage('build') {
            steps {
                echo 'Building application'
            }
        }
        
        stage('test'){
            steps {
                echo 'Testing application.'
            }
        }
        
        stage('deploy'){
            steps {
                echo 'Deploying application.'
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
