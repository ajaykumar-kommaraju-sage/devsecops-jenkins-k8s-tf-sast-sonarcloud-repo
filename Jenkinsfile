pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=ajaythesrewebapp -Dsonar.organization=ajaythesrewebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=83c78f4bedc58f9932a8bd080755145eca835617'
			}
        } 
  }
}
