pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=testbuggycodefordevsecopskurs -Dsonar.organization=testbuggycodefordevsecopskurs -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=6ea25115076de6a3199aeeed224152d574e8a51d'
			}
        } 
  }
}
