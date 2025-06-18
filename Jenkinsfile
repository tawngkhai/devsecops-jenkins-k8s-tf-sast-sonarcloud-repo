pipeline {
  agent any
  tools {
        maven 'maven3'
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {
                sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=buggywebap -Dsonar.organization=buggywebap -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=9fe9a045d27d5db886581092dffc8e53f742c99d'
                        }
        }
  }
}
