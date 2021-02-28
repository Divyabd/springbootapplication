
pipeline{
   agent  {
    docker {  
      image 'maven:3.6.3-jdk-11'
      args '-v /root/.m2:/root/.m2'
     
    }
  }

stages{
    stage('maven validate'){
        steps{
          sh 'mvn validate'
        }
    }
}

    stage('maven compile'){
        steps{
          sh 'mvn compile'
        }
    }

    stage('maven install'){
        steps{
          sh 'mvn install'
        }
    }

    stage('maven package'){
        steps{
          sh 'mvn package'
        }
    }


}