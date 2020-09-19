pipeline{
    agent any
    stages{
        stage ('Build')
        {
            steps{
                script {
			def workspace = pwd()
			}
		echo 'first build'
		sh "echo ${workspace}" 
		sh "chmod 777 ${workspace}"
		
		sh "docker build -t test1.0 ."	    
		echo 'first build'
		   }
		
        }
            stage ('Deploy')
        {
            steps{
                echo 'first build'
            }

        }
    }
    
}
