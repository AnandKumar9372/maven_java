pipeline{
  agent any
  stages{
    stage("Bulid"){
      steps{
          echo 'building the project'
          sh 'mvn validate'
    }
     stage("test"){
       steps{
          echo 'testing the project '
          sh 'mvn compile'
          sh 'mvn test'
       }
    }
     stage("deploy"){
       steps{
          echo 'deploying the project '
          sh 'mvn package'
       }
    }
  }
}
