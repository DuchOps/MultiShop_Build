node {
 stage ('Checkout')  {

     build job: 'CheckOut' 
 }
stage ('Build') {
     build job: 'Build' 
    }
stage ('Code Quality scan') {
      build job: 'Code_Quality' 
        }
        
stage('Archive Artifacts') {
build job: 'Archive_Artifacts'
}
 stage('Publish to Artifactory') {
build job: 'Publish_To_Artifactory'
}

stage ('Slack notification') {
     
build job: 'Slack_Notification'
    }
  
}