pipeline {
    agent any
    tools{
        maven 'localmvn'    
    }
    stages {
        stage('Build') {
            steps {
              bat 'mvn clean'
            }
        }
        stage('Compile') {
            steps {
               bat 'mvn compile'
            }
        }
        stage('Test') {
            steps {
               bat 'mvn test'
            }
        }
        stage('Package') {
            steps {
               bat 'mvn package'
            }
        }
    }
}
   
