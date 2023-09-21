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
   agent { label 'luckynode' }
   steps
   {
   sh "mvn compile"
    sh "mvn test"
    sh "mvn package"
   }
  }
 }
}
