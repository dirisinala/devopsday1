pipeline{
    agent any
    stages{
        stage('gitcheckout'){
            steps{
            echo 'first clone'
                
            }
        }
        stage ('Sonar')
        {
            steps{
                withSonarQubeEnv{
                sh “/var/lib/jenkins/hudson.plugins.sonar.SonarRunnerInstallation/sonarqubescanner/bin/sonar-scanner -Dsonar.host.url=http://phaniavula.eastus.cloudapp.azure.com:9000/ -Dsonar.projectName=meanstackapp -Dsonar.projectVersion=1.0 -Dsonar.projectKey=meanstack:app -Dsonar.sources=. -Dsonar.projectBaseDir=/home/jenkins/workspace/sonarqube_test_pipeline"22:16
                sh “/var/lib/jenkins/hudson.plugins.sonar.SonarRunnerInstallation/sonarqubescanner/bin/sonar-scanner -Dsonar.host.url=http://phaniavula.eastus.cloudapp.azure.com:9000/ -Dsonar.projectName=meanstackapp -Dsonar.projectVersion=1.0 -Dsonar.projectKey=meanstack:app -Dsonar.sources=. -Dsonar.projectBaseDir=/home/jenkins/workspace/sonarqube_test_pipeline"22:16
            }
        }
           
    }
}
