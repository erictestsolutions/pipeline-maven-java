pipeline{
    agent any
    
    stages{        
        stage("Compile"){
            steps{
                bat "mvn compile"
            }
        }
        
        stage("Test"){
            steps{
                bat "mvn test"
            }
        }
        
        stage("Build"){
            steps{
                bat "mvn package"
            }
        }
        
        stage("Deploy"){
            steps{
                bat 'java -cp target/your-app-1.0-SNAPSHOT.jar com.apasoft.ToUpper "%TEXT%"'
            }
        }
    }
}
