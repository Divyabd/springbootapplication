
pipeline{
   agent  {
    docker {  
      image 'maven:3.6.3-jdk-11'
      args '-v /root/.m2:/root/.m2'
     
    }
  }

stages{
    stage('maven clean'){
        steps{
          sh 'mvn clean'
        }
    }
}
}