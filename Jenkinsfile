pipeline{
    agent any
    stages{
        stage ('Build')
        {
            steps{
                echo 'first build'
		def workspace = pwd()
		sh 'echo ${workspace}' 
		sh 'docker build -t test1.0 .'	    
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
