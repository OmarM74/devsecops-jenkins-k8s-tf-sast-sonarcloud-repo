pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=buggywebapportest -Dsonar.organization=DevSecOpsKurs -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=c484b7490ba40e8c1406f78089fe56039b6c46eb'
			}
        } 
  }
}
