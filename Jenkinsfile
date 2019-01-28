pipeline {

    agent any
    tools {
        maven 'maven_3' 
    }
    stages {
        stage('Compile stage') {
            steps {
                bat "mvn clean compile" 
        }
    }

         stage('Database Deployment') {
             steps {
                bat "mvn test"
        }
    }

          stage('Code Test') {
              steps {
                bat "mvn clean compile"
        }
    }
        stage('Code Deployment') {
              steps {
                bat "mvn clean compile"
        }
    }

  }

}
