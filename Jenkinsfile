pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=buggywebapp01 -Dsonar.organization=buggywebapp01 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=0883fa632f7e6b850488de21d78e34d949e5b8a0'
			}
        } 
  }
}
