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
                 echo "JAVA_HOME = %JAVA_HOME%"
                  echo "MAVEN_HOME = %JAVA_HOME%"
                '''
            }
        }
           stage ('Testing clean') {

            steps {
               // withMaven(maven : 'maven_3.6.0') {
               //     sh 'mvn test'
               // }
                 bat 'mvn clean'
                 echo "hello Testng Stage"
            }
        }
        
         stage ('Testing Stage') {

            steps {
               // withMaven(maven : 'maven_3.6.0') {
               //     sh 'mvn test'
               // }
              //   bat 'mvn test'
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
