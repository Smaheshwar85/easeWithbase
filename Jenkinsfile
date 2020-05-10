node{
   stage('SCM Checkout'){
     git 'https://github.com/Smaheshwar85/easeWithbase'
   }
   stage('Compile-Package'){
      def mvnHome =  tool name: 'maven3', type: 'maven'   
      sh "${mvnHome}/bin/mvn package"
    sh 'mvn package'
   }
}
