
pipeline{
    agent any
// uncomment the following lines by removing /* and */ to enable
    tools{
       nodejs 'Maven 3.6.3' 
    }
    
    stages{
        stage('build'){
            steps{
                echo 'this is the buildjob'
                sh 'npm install'
         
            }
        }
        stage('test'){
            steps{
                echo 'this is the test job'
                sh 'npm'
         
            }
        }
        stage(packge'){
            steps{
                echo 'this is the package job'
                sh 'npm run package'
                
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline has completed...'
        }
        
    }
    
}
