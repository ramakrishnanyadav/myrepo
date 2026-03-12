pipeline 
{
agent any
stages{
    stage('Checkout')
      {
      steps {'https://github.com/ramakrishnanyadav/myrepo.git'}
      }
    stage ('Publish'){
      steps {
        publishHTML([
          allowMissing:true,
          alwaysLinkToLastBuild:false,
          keepAll:false,
          reportDir:'.',
          reportFiles:'Index.html' ,
          reportName:'My html report' 
        ])
      }
    }
  }

}
