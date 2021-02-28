
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
stages{
    stage('maven compile'){
        steps{
          sh 'mvn compile'
        }
    }
}
stages{
    stage('maven install'){
        steps{
          sh 'mvn install'
        }
    }
}
stages{
    stage('maven package'){
        steps{
          sh 'mvn package'
        }
    }
}

}