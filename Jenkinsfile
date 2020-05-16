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
   emailext body: '''Thanks & Regards,
Shantu Kumar''', subject: 'Jenkins-pipeline-Project', to: 'softwareshut@gmail.com'
    }
  }
