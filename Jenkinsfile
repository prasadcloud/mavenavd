@Library('mylibrary')_
node('built-in')
{
    
        stage('Continous Download')
        {
            
                
                    cicdavd.contDownload("mavenavd.git")
                
            
        }
         stage('Continous Build')
        {
            
                
                    cicdavd.contBuild()
              
        }
         stage('Continous Deploy')
        {
            
                    cicdavd.contDep("SharedPipelineLibrary1", "172.31.26.206", "testavd2")
        }
         stage('Continous Testing')
        {
            
                    cicdavd.contDownload("FunctionalTesting.git")
                    cicdavd.contTest("SharedPipelineLibrary1")
              
        }
         stage('Continous Delivery')
        {
            
                    cicdavd.contDep("SharedPipelineLibrary1", "172.31.21.142", "prodavd2")
              
        }

}
