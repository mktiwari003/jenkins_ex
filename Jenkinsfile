pipeline {
    agent any
      tools {
        maven 'maven_3.6.0' 
    }
    stages {
        stage ('Compile Stage') {

            steps {
              //  withMaven(maven : 'maven_3.6.0') {
               //     bat 'mvn clean compile'
               // }
                echo "hello Compile Stage"
                echo "PATH = %PATH%"
                
                bat '''
                 echo "PATH = %PATH%"
                 echo "MVN_HOME = %MVN_HOME%"
                '''
            }
        }
           stage ('Testing Stage') {

            steps {
               // withMaven(maven : 'maven_3.6.0') {
               //     sh 'mvn test'
               // }
                 bat 'mvn test'
                 echo "hello Testng Stage"
            }
        }


        stage ('Deployment Stage') {
            steps {
             ////   withMaven(maven : 'maven_3.6.0') {
                  //  sh 'mvn deploy'
              //  }
                
                 echo "hello Deployment Stage"
            }
        }
       
    }
}
