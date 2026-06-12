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
steps{step{checkout scm}}
stage('B&T')
{
steps{step{sh 'mvn clean install'}}
stage('run')
{
steps{step{sh 'java -jar target/*.jar'}}
}}}}}
