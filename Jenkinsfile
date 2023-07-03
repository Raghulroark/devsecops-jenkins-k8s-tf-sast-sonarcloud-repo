pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=Raghulbuggyapp -Dsonar.organization=Raghulbuggyapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=3e2ef39aa66f57eb8291ff0571a1e769755a0af5'
			}
        } 
  }
}
