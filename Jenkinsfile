jenkins webhook integration with github 

node{
   stage('SCM Checkout'){
     git 'https://github.com/ankittomar0207/Demojenkins/'
   }
   stage('Deploy to Tomcat'){
      
     sshagent(['tomcat-dev']) {
  sh 'scp -o StrictHostKeyChecking=no tmp/*.war root@10.67.174.55:/opt/local/tomcat/webapps/'
  
}
     
   }
