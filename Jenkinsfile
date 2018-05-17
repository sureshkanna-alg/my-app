node{
   stage('SCM Checkout.'){
     git 'https://github.com/sureshkanna-alg/my-app'
   }
   stage('Compile-Package'){
      // Get maven home path 
      def mvnHome = tool name: 'maven-3.3.9', type: 'maven'
      sh "${mvnHome}/bin/mvn clean package"
   }
   stage('Deploy on Tomcat'){
      sh "cp /var/lib/jenkins/workspace/my-app/target/myweb-0.0.1.war /opt/tomcat8/webapps"
   }
      
}
