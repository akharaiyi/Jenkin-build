pipeline {
     agent  any  //{ label 'java' } 
    stages {
        stage('Build') { 
            steps {
              sh "mvn clean"
            }
        }
        stage('Test') { 
            steps {
               sh "mvn test"
               
               
            }
        }
        stage('package') { 
            steps {
                sh " mvn package" 
                sh "ps -ef"
                sh "java -version"
            }
        }
        stage('deploy'){
            steps{
              echo "deploy to tomcat server on ec2"   
            }
        }
    }
}
