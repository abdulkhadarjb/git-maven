node {
    stage('Git'){
      git 'https://github.com/abdulkhadarjb/webfiles.git'      
    }
    
    stage('Maven Build'){
      sh 'mvn clean package'   
    }
    stage('Archive Artifacts'){
         archiveArtifacts 'target/myweb.war'
    }
    
    stage('Email'){
    
    mail bcc: '', body: '''Thanks,
Java Home''', cc: '', from: '', replyTo: '', subject: 'Pipeline Demo', to: 'skabdul.marolix@gmail.com'





    }
}
