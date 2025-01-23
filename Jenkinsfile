pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp -Dsonar.organization=asgbuggywebapp -
	Dsonar.host.url=https://sonarcloud.io -Dsonar.token=69d984d2f8dd1a661f3a53f4eebb5e0e180b34ca'
			}
        } 
  }
}
