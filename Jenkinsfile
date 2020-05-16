node{
    stage('SCM Checkout'){
     git 'https://github.com/shantusanay/Jenkins-project1'
     }
     
    stage('Compile Package'){
        //Get Maven Path
        def mvnHome = tool name: 'maven-3', type: 'maven'
        sh "${mvnHome}/bin/mvn package"
     }
  }
