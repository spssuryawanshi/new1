pipeline {

 agent any

     stages {

         stage ('git fetch') {
        
           steps {
                 git branch: 'main', url: 'https://github.com/spssuryawanshi/new1.git'
                  }

             }
       

         stage ('store to S3') {
          steps {
                script {
                    // Assuming you have AWS CLI installed and configured on your Jenkins instance
                    sh 'aws s3 cp . s3://mybucket2463/ --recursive'
                }
            }
        }
    }
}
        
           
      
        

      
