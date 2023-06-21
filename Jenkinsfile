pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
 tools{
       nodejs ‘nodejs’ 
    }
 

    stages{
        stage('build-the-app'){
            steps{
                echo 'build the job app'
                sh 'npm install'
                sleep 4
            }
        }
        stage('test-the-app'){
            steps{
                echo 'test the app'
                sh 'npm test'
                sleep 9
            }
        }
        stage('package-the-app'){
            steps{
                echo 'package the app'
                sh 'npm package'
                sleep 7
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline has completed...'
        }
        
    }
    
}
