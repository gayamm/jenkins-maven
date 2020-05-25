node{
stage('SCM Checkout')
{
git 'https://github.com/gayamm/jenkins-maven'
}
stage('Compile-Package')
{
  //Get maven home path
  def mvnHome= tool name: 'Maven-aws', type: 'maven'
  sh "${mvnHome}/bin/mvn package"
}
}
