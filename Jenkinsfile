pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=bsgbuggywebapp -Dsonar.organization=bsgbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=8644c4a097a03868ee730892dd8322204fd126b8'
			}
        } 
  }
}
