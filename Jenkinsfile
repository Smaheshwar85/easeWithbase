node{
   stage('SCM Checkout'){
     git 'https://github.com/Smaheshwar85/easeWithbase'
   }
   stage('Compile-Package'){
      def mvnHome =  tool name: 'Mavan3', type: 'maven'
      sh "${mvnHome}/bin/mvn package"
   
     }
    stage('Email Notification'){
      mail bcc: '', body: '''Hi Welcome to jenkins email alerts
      Thanks
      Mahesh''', cc: '', from: '', replyTo: '', subject: 'Jenkins Job', to: 'smahesh2305@gmail.com'
   }
}
