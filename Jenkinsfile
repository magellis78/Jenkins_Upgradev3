node('master')
{
   stage('ContinuousDownload') 
       {
        https://github.com/magellis78/Jenkins_Upgradev3.git  
        }
            
         stage('ContinuousBuild')
         {
          sh 'mvn package'
          }
     stage('Deploy') 
          {
           scp/home/ubuntu/.jenkins/workspace/scriptedPipeline/webapp/target/webapp.war ubuntu@172.31.80.201:/var/lib/tomcat9/webapps/testapps.war
           }
            stage('Deploy Production') 
            {
             scp/home/ubuntu/.jenkins/workspace/scriptedPipeline/webapp/target/webapp.war ubuntu@172.31.80.246:/var/lib/tomcat9/webapps/testapps.war
 
             }
            }
      }
}
