node{
    stage('SCM Checkout'){
     git 'https://github.com/shantusanay/Jenkins-project1'
     }
     
    stage('Compile Package'){
        //Get Maven Path
        def mvnHome = tool name: 'maven-3', type: 'maven'
        sh "${mvnHome}/bin/mvn package"
     }
    stage('Email Notification'){
        mail bcc: '', body: '''Thanks & Regards,
Shantu Kumar S''', cc: '', from: '', replyTo: '', subject: 'Jenkins Project', to: 'softwareshut@gmail.com'
    }
  }
