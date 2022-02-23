pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
    tools{
       nodejs 'nodejs' 
    }
    

    stages{
        stage('compile-app'){
            steps{
                echo 'this is the compile job'
                sh 'npm install'
            }
        }
        stage('test-app'){
            steps{
                echo 'this is the test job'
                sh 'npm test'
            }
        }
        stage('package-app'){
            steps{
                echo 'this is the package job'
                sh 'npm package'
            }
        }
    }
    
    post{
        always{
            echo 'My first code pipeline ...this pipeline has completed...'
        }
        
    }
    
}
