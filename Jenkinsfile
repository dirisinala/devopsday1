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
		sh "docker images"
		sh "docker ps"
		sh "docker ps -a"
		sh "docker run prime1.0"
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
