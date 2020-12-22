pipeline {
    agent any
     environment {
        PATH = "/opt/maven/apache-maven-3.6.3/bin:$PATH"
    }

    stages {
        stage('build') {
            steps {
                sh 'mvn clean compile '
            }
        }
        stage('test') {
            steps {
                sh 'mvn test '
            }
        }
    }

}
