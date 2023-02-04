pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
   tools{
       maven  'maven' 
    }
    

    stages{
        stage('build the app'){
            steps{
                echo 'this is the build job'
                sh 'mvn compile'
                  }
        }
        stage('test the app'){
            steps{
                echo 'this is the test job'
                sh 'mvn test'
               
            }
        }
        stage('package the app'){
            steps{
                echo 'this is the pakage job'
                sh 'mvn package -DskipTests'
               
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline has completed...'
        }
        
    }
    
}


