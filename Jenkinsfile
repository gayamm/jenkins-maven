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
  stage('Email Notification')
  {
    mail bcc: '', body: '''Hi 

Hi this is test email pipeline from jenkins.

Regards
Mahesh G''', cc: '', from: '', replyTo: '', subject: 'Jenkins Maven email', to: 'maheswarareddy.gm@gmail.com'
  }
}
