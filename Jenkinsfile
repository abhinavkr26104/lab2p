pipeline
{
agent any
tools
{
maven 'Maven'
}
stages
{
stage('checkout')
{
steps
  {
    checkout scm
  }
  }
stage('B&T')
{
steps
  {
  
      sh 'mvn clean install'
    }
  }
stage('run')
{
steps
  {
    
      sh 'java -jar target/*.jar'
  }
  
  }
}
}
