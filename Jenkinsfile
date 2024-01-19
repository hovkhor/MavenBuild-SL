pipeline{
    
    tools{
        maven 'mymaven'
    }
    
    // where to run the pipeline
    // agent means a server/virtual machine
    // any here means--current windows server
    agent any
    
    // In pipline we want to exeucte many jobs -> called stages
    // pipeline = set of stages/set of task
    
    stages{
        
        // each task/job represents a stage
        
        stage('Clone the repo'){
            steps{
              git 'https://github.com/Sonal0409/ATE_Phase2-Selenium-Jenkins-Jan24.git'  
            }
        }

      stage('Compile the code'){
            steps{
            sh 'mvn test'  
            //bat :  you are running the command using windows command line(batch)
            }
        }
        
        stage('Execute the tests'){
            steps{
            sh 'mvn test'  
            //bat :  you are running the command using windows command line(batch)
            }
        }

        stage('Execute the package'){
            steps{
            sh 'mvn package'  
            //bat :  you are running the command using windows command line(batch)
            }
        }
        
    }
       
}
