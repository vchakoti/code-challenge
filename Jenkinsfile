pipeline
{
agent any
	tools 
	{
		maven 'my_local_maven'
	}
  stages 
  {
  stage ('build my applicaiton')
  {
   steps{
   bat 'mvn clean package'
   // sh 'mvn clean package'
   
   }
  }
   stage ('Test my applicaiton')
  {
   steps{
   bat 'mvn test'
   // sh 'mvn clean package'
   
   }
 
  }
  stage ('deploy my applicaiton to cloud')
  {
   steps{
   bat 'mvn package deploy -DmuleDeploy'
   // sh 'mvn clean package'
   
   }
 
  }
    
}