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
            environment { 
                def scannerHome = tool name: 'SonarQubeScanner', type: 'hudson.plugins.sonar.SonarRunnerInstallation'; } 
            steps { 
                withSonarQubeEnv('SonarQubeServer') { sh "${scannerHome}/bin/sonar-scanner -Dsonar.projectKey=CSS_API_Policy -Dsonar.exclusions=appdynamics/** -Dsonar.jacoco.reportPaths=build/jacoco/test.exec -Dsonar.junit.reportPaths=build/test-results/test -Dsonar.java.binaries=./src/main/** -Dsonar.sources=src" } } }
            steps{
                withSonarQubeEnv{
                sh “/var/lib/jenkins/hudson.plugins.sonar.SonarRunnerInstallation/sonarqubescanner/bin/sonar-scanner -Dsonar.host.url=http://phaniavula.eastus.cloudapp.azure.com:9000/ -Dsonar.projectName=meanstackapp -Dsonar.projectVersion=1.0 -Dsonar.projectKey=meanstack:app -Dsonar.sources=. -Dsonar.projectBaseDir=/home/jenkins/workspace/sonarqube_test_pipeline"22:16
                            }
        }
           
    }
}
