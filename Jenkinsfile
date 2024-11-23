pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=final-capstone-lavanya_sample-code -Dsonar.organization=final-capstone-lavanya -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=2ad436d1a5c2d1e6a95d1301bdba9f5efe177e37'
			}
        } 
  }
}
