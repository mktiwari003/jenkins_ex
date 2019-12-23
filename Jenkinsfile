pipeline {
    agent any
      tools {
        maven 'maven_3.6.0' 
    }
    stages {
        stage ('Compile Stage') {

            steps {
                withMaven(maven : 'maven_3.6.0') {
                    bat 'mvn clean compile'
                }
            }
        }

       
    }
}
