pipeline {
	
	environment {
    GIT_URL="https://github.com/MishraKD/assignment11.git"
   
		
	}
	
agent any	
	stages{
            
stage('DeployToProduction') {
	
             steps {
		      git url: "${GIT_URL}"
		     
		kubernetesDeploy(
		     
		    
                    //credentialsType: 'KubeConfig',
                    kubeconfigId: 'kubeconfiggit',
                    //kubeConfig: [path: '/var/jenkins_home/workspace/.kube/config'],
                    configs: 'deploymentfile.yml',

                    enableConfigSubstitution: true   
             )
			 
			   
		}
	     }
	}
}
		

		
		        

		

					    

			 



  
	
