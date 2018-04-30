node{
   stage('SCM Checkout'){
     git 'https://github.com/sureshkanna-alg/my-app'
   }
   stage('Compile-Package'){
      // Get maven home path   
      sh 'mvn clean package'
   }
}
