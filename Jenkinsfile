pipeline {
  agent any
  tools { 
        maven 'maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=joebuggywebapp1 -Dsonar.organization=joebuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=c615a053e5acf54ba3bc04307a9bda446a09f7dc'
			}
        } 
  }
}
