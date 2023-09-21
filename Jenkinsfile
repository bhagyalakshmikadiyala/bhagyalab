pipeline
{
agent any
stages
 {
 stage('validate')
 {
 steps
  {
 sh "mvn validate"
  }
 }
  stage('Build')
  {
   steps
   {
   sh "mvn compile"
    sh "mvn test"
    sh "mvn package"
   }
  }
 }
}
