pipeline {
    
agent any
    environment {
        PATH = "/opt/maven/apache-maven-3.6.3/bin:$PATH"
    }
    stages {  
        stage('Build Stage') { 
            steps { 
                {
                    sh 'mvn clean compile '
                }
                  
                   echo 'Running on build stage '
            }
        }
        stage('Test Stage') { 
            steps {
                {
                    sh 'mvn test '
                }
                      echo 'Running on test stage '
                
            }
        }
        
    }
}
