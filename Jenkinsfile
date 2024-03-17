pipeline {
    agent any 

    stages {
        stage('Checkout') {
            steps {
                     checkout scm
                  }
                          }
        stage('Build') {
            steps {
                    sh '/home/snehal/Documents/Extract/apache-maven-3.9.6/bin/mvn install'
                  }
                       }
        stage('Deployment') {
            steps {
                    sh 'cp target/prod1.war /home/snehal/Documents/Extract/apache-tomcat-9.0.86/webapps'
                  }
                            }

           }
        }
            
