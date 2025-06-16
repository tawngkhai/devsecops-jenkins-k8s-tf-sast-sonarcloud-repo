pipeline {
  agent any
  tools {
        maven 'Maven3'
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {
                sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=buggywebapp -Dsonar.organization=buggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=388c4910c754ca93a55d9b7b58aedc38e8681084'
                        }
        }
  }
}
