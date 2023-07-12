pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=kwebapp -Dsonar.organization=kwebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=81fea981c63ada79a1483306b84ad8e9c54c491e'
			}
        } 
  }
}
