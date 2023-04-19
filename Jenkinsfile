pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asecuritybuggywebapp -Dsonar.organization=asecuritybuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=66e701eb978c584ec87d415e79f94092260a88e7'
			}
        } 
  }
}
