pipeline {
      agent any
      stages {
            stage('Init') {
                  steps {
                        echo 'Hi, this is Anshul from LevelUp360'
                        echo 'We are Starting the Testing'
                  }
            }
            stage('Build') {
                  steps {
                        echo 'Building Sample Maven Project'
                  }
            }
            stage('Deploy') {
                  steps {
                        scp/home/ubuntu/.jenkins/workspace/scriptedPipeline/webapp/target/webapp.war ubuntu@172.31.80.201:/var/lib/tomcat9/webapps/testapps.war
                        {
            }
            stage('Deploy Production') {
                  steps {
                        scp/home/ubuntu/.jenkins/workspace/scriptedPipeline/webapp/target/webapp.war ubuntu@172.31.80.246:/var/lib/tomcat9/webapps/testapps.war
 
                        }
            }
      }
}
