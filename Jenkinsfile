pipeline {
    agent any
      tools {
        maven 'maven_3.6.0' 
    }
    stages {
        stage ('Compile Stage') {

            steps {
                withMaven(maven : 'maven_3.6.0') {
                    sh 'mvn clean compile'
                }
            }
        }

        stage ('Testing Stage') {

            steps {
                withMaven(maven : 'maven_3.6.0') {
                    sh 'mvn test'
                }
            }
        }


        stage ('Deployment Stage') {
            steps {
                withMaven(maven : 'maven_3.6.0') {
                    sh 'mvn deploy'
                }
            }
        }
    }
}
